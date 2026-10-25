# numbers.md

GPU specs for P0. Every number was checked against NVIDIA's own pages.

| Spec | T4 | H100 SXM | Source |
|---|---|---|---|
| Memory (GB) | 16 | 80 | datasheets below |
| Bandwidth (GB/s) | 320 | 3,350 | datasheets below |
| FP16 TFLOPS (dense, tensor cores) | 65 | ~989 | datasheets below |
| Power (W) | 70 | 700 | datasheets below |

Sources:
- T4: [T4 datasheet (PDF)](https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/tesla-t4/t4-tensor-core-datasheet-951643.pdf)
- H100: [H100 specs](https://www.nvidia.com/en-us/data-center/h100/) (SXM column)

Notes:
- T4 "32 GB/s" on the datasheet is the PCIe link to the CPU, not GPU memory bandwidth (320 GB/s).
- T4 8.1 TFLOPS is FP32 (single precision). FP16 mixed precision on tensor cores is 65.
- H100 FP16 is listed as 1,979 TFLOPS *with sparsity*. Dense is half: ~989.

## Prediction

_TODO (Sunny): write the T4 1.5B decode ceiling math in your own words, plus the H100 ceiling._
