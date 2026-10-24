vLLM on a T4

Benchmarking vLLM serving a small model on an NVIDIA T4 GPU.

## Done when (Nov 15, 2026)
- Fixed model + GPU
- ≥3 request rates × 2 prompt/output lengths
- TTFT (time to first token), p50 / p95 latency
- Compared with the memory-bandwidth ceiling
- One command reproduces it
- Raw JSON results committed

## Results
| Request rate | Length | TTFT p50 | TTFT p95 | Latency p50 | Latency p95 | tok/s |
|---|---|---|---|---|---|---|
| | | | | | | |
