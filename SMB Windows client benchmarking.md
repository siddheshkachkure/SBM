# SMB-W Storage Benchmark Guide for Windows - shared storage drive (SAMBA)
> FIO-based comprehensive storage benchmarking for SMB storage attached via SMB-W as a network drive on Windows nodes.

---

## Prerequisites

- FIO installed on Windows
- Weka storage mounted as a network drive (e.g., `Z:`)
- Run **all commands from the Windows render node** with the SMB share mounted
- Create the test directory before starting:

```cmd
mkdir Z:\fio_bench
```

---

## Test Overview

| # | Test | Block Size | Pattern | Purpose |
|---|------|-----------|---------|---------|
| 1 | Sequential Write | 1M | Write | Render output / EXR frame writes |
| 2 | Sequential Read | 1M | Read | Scene/asset loading |
| 3 | Sequential Mixed | 1M | 70R/30W | Concurrent read-write workload |
| 4 | Sequential Write | 128K | Write | Simulation / cache file writes |
| 5 | Sequential Read | 128K | Read | Medium block read throughput |
| 6 | Random Write | 4K | Write | Metadata / small file stress |
| 7 | Random Read | 4K | Read | Texture / cache random access |
| 8 | Random Mixed | 4K | 70R/30W | Mixed small I/O workload |
| 9 | Random Read | 64K | Read | Shader / HDR texture access |
| 10 | Random Write | 64K | Write | Medium random write |
| 11 | Queue Depth Scaling | 1M | Read | QD1 → QD128 concurrency ramp |
| 12 | Multi-Job Concurrency | 1M | Read | Simulates multiple render nodes |
| 13 | Render Frame Write | 4M | Write | Individual frame file simulation |
| 14 | Latency Benchmark | 4K | Rand Read | Latency-sensitive operation baseline |
| 15 | Endurance Test | 1M | 50R/50W | Long-duration sustained throughput |

---

## Key FIO Parameters

| Parameter | Value | Reason |
|-----------|-------|--------|
| `--ioengine` | `windowsaio` | Native async I/O for Windows — mandatory for SMB |
| `--direct` | `1` | Bypasses Windows file cache — tests true Weka performance |
| `--iodepth` | `32–128` | Controls outstanding concurrent I/O queue depth |
| `--numjobs` | `4–16` | Parallel workers simulating render processes |
| `--time_based` | — | Fixed duration run instead of fixed data size |
| `--group_reporting` | — | Aggregates all job stats into single summary |
| `--runtime` | `120` | 2 min per test (increase to `300` for production runs) |
| `--percentile_list` | `50:90:95:99:99.9` | Full latency percentile breakdown |

---

## Tests

### 1. Sequential Write — 1M Block (Render Output)

```cmd
fio --name=seq_write_large --ioengine=windowsaio --iodepth=32 --rw=write --bs=1M --direct=1 --size=32G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\seq_write_large.dat --output=Z:\fio_bench\result_seq_write_large.txt
```

---

### 2. Sequential Read — 1M Block (Asset Loading)

```cmd
fio --name=seq_read_large --ioengine=windowsaio --iodepth=32 --rw=read --bs=1M --direct=1 --size=32G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\seq_write_large.dat --output=Z:\fio_bench\result_seq_read_large.txt
```

---

### 3. Sequential Mixed Read/Write — 1M Block (70/30)

```cmd
fio --name=seq_rw_mixed_large --ioengine=windowsaio --iodepth=32 --rw=rw --rwmixread=70 --bs=1M --direct=1 --size=32G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\seq_rw_mixed.dat --output=Z:\fio_bench\result_seq_rw_mixed_large.txt
```

---

### 4. Sequential Write — 128K Block (Cache Files)

```cmd
fio --name=seq_write_128k --ioengine=windowsaio --iodepth=32 --rw=write --bs=128K --direct=1 --size=16G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\seq_write_128k.dat --output=Z:\fio_bench\result_seq_write_128k.txt
```

---

### 5. Sequential Read — 128K Block

```cmd
fio --name=seq_read_128k --ioengine=windowsaio --iodepth=32 --rw=read --bs=128K --direct=1 --size=16G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\seq_write_128k.dat --output=Z:\fio_bench\result_seq_read_128k.txt
```

---

### 6. Random Write — 4K (Metadata / Small File Stress)

```cmd
fio --name=rand_write_4k --ioengine=windowsaio --iodepth=64 --rw=randwrite --bs=4K --direct=1 --size=8G --numjobs=8 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\rand_write_4k.dat --output=Z:\fio_bench\result_rand_write_4k.txt
```

---

### 7. Random Read — 4K (Texture / Cache Access)

```cmd
fio --name=rand_read_4k --ioengine=windowsaio --iodepth=64 --rw=randread --bs=4K --direct=1 --size=8G --numjobs=8 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\rand_write_4k.dat --output=Z:\fio_bench\result_rand_read_4k.txt
```

---

### 8. Random Mixed Read/Write — 4K (70/30)

```cmd
fio --name=rand_rw_4k --ioengine=windowsaio --iodepth=64 --rw=randrw --rwmixread=70 --bs=4K --direct=1 --size=8G --numjobs=8 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\rand_rw_4k.dat --output=Z:\fio_bench\result_rand_rw_4k.txt
```

---

### 9. Random Read — 64K (Shader / HDR Texture)

```cmd
fio --name=rand_read_64k --ioengine=windowsaio --iodepth=32 --rw=randread --bs=64K --direct=1 --size=16G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\rand_read_64k.dat --output=Z:\fio_bench\result_rand_read_64k.txt
```

---

### 10. Random Write — 64K

```cmd
fio --name=rand_write_64k --ioengine=windowsaio --iodepth=32 --rw=randwrite --bs=64K --direct=1 --size=16G --numjobs=4 --runtime=120 --time_based --group_reporting --filename=Z:\fio_bench\rand_write_64k.dat --output=Z:\fio_bench\result_rand_write_64k.txt
```

---

### 11. Queue Depth Scaling — Sequential Read (QD1 → QD128)

```cmd
fio --name=seq_qd1 --ioengine=windowsaio --iodepth=1 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\qd_test.dat --output=Z:\fio_bench\result_qd1.txt

fio --name=seq_qd4 --ioengine=windowsaio --iodepth=4 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\qd_test.dat --output=Z:\fio_bench\result_qd4.txt

fio --name=seq_qd16 --ioengine=windowsaio --iodepth=16 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\qd_test.dat --output=Z:\fio_bench\result_qd16.txt

fio --name=seq_qd32 --ioengine=windowsaio --iodepth=32 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\qd_test.dat --output=Z:\fio_bench\result_qd32.txt

fio --name=seq_qd64 --ioengine=windowsaio --iodepth=64 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\qd_test.dat --output=Z:\fio_bench\result_qd64.txt

fio --name=seq_qd128 --ioengine=windowsaio --iodepth=128 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\qd_test.dat --output=Z:\fio_bench\result_qd128.txt
```

---

### 12. Multi-Job Concurrency Scaling (Simulating Multiple Render Nodes)

```cmd
fio --name=concur_1j --ioengine=windowsaio --iodepth=16 --rw=read --bs=1M --direct=1 --size=8G --numjobs=1 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\concur_1j.dat --output=Z:\fio_bench\result_concur_1j.txt

fio --name=concur_4j --ioengine=windowsaio --iodepth=16 --rw=read --bs=1M --direct=1 --size=8G --numjobs=4 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\concur_4j.dat --output=Z:\fio_bench\result_concur_4j.txt

fio --name=concur_8j --ioengine=windowsaio --iodepth=16 --rw=read --bs=1M --direct=1 --size=8G --numjobs=8 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\concur_8j.dat --output=Z:\fio_bench\result_concur_8j.txt

fio --name=concur_16j --ioengine=windowsaio --iodepth=16 --rw=read --bs=1M --direct=1 --size=8G --numjobs=16 --runtime=60 --time_based --group_reporting --filename=Z:\fio_bench\concur_16j.dat --output=Z:\fio_bench\result_concur_16j.txt
```

---

### 13. Render Frame Write Pattern (Many Files Simulation)

```cmd
fio --name=render_frame_write --ioengine=windowsaio --iodepth=8 --rw=write --bs=4M --direct=1 --size=512M --numjobs=8 --nrfiles=100 --file_service_type=sequential --openfiles=8 --runtime=120 --time_based --group_reporting --directory=Z:\fio_bench\ --output=Z:\fio_bench\result_render_frame_write.txt
```

---

### 14. Latency Benchmark — Low QD Random Read

```cmd
fio --name=latency_rand_read --ioengine=windowsaio --iodepth=1 --rw=randread --bs=4K --direct=1 --size=4G --numjobs=1 --runtime=60 --time_based --percentile_list=50:90:95:99:99.9 --group_reporting --filename=Z:\fio_bench\latency_test.dat --output=Z:\fio_bench\result_latency_rand_read.txt
```

---

### 15. Sustained Throughput Endurance Test (10 Minutes)

```cmd
fio --name=endurance_seq_rw --ioengine=windowsaio --iodepth=32 --rw=rw --rwmixread=50 --bs=1M --direct=1 --size=64G --numjobs=4 --runtime=600 --time_based --group_reporting --filename=Z:\fio_bench\endurance.dat --output=Z:\fio_bench\result_endurance.txt
```

---

## Reading Results

In each output `.txt` file look for these key metrics:
bw=XXXXX KiB/s        → Throughput (bandwidth)
iops=XXXX             → I/O Operations per second
lat (usec/msec)       → Latency (avg, min, max)
clat percentiles      → P50 / P90 / P99 / P99.9 latency

---

## Cleanup After Testing

```cmd
del /Q Z:\fio_bench\*.dat
rmdir Z:\fio_bench
```

---

## Important Notes

- Always use `--ioengine=windowsaio` — do **not** use `sync` or `libaio` on Windows SMB
- `--direct=1` is mandatory to bypass Windows cache and test actual Weka storage
- Always **pre-write data first** before running any read tests (the write test creates the `.dat` file the read test uses)
- Run a **baseline test during off-peak hours** before testing under active render load
- For production benchmarking, increase `--runtime` from `120` to `300` seconds per test
- All result files are saved to `Z:\fio_bench\result_*.txt`

---

## Result Files Reference

| File | Test |
|------|------|
| `result_seq_write_large.txt` | Sequential Write 1M |
| `result_seq_read_large.txt` | Sequential Read 1M |
| `result_seq_rw_mixed_large.txt` | Sequential Mixed 1M |
| `result_seq_write_128k.txt` | Sequential Write 128K |
| `result_seq_read_128k.txt` | Sequential Read 128K |
| `result_rand_write_4k.txt` | Random Write 4K |
| `result_rand_read_4k.txt` | Random Read 4K |
| `result_rand_rw_4k.txt` | Random Mixed 4K |
| `result_rand_read_64k.txt` | Random Read 64K |
| `result_rand_write_64k.txt` | Random Write 64K |
| `result_qd1.txt` → `result_qd128.txt` | Queue Depth Scaling |
| `result_concur_1j.txt` → `result_concur_16j.txt` | Concurrency Scaling |
| `result_render_frame_write.txt` | Render Frame Pattern |
| `result_latency_rand_read.txt` | Latency Benchmark |
| `result_endurance.txt` | Endurance Test |
