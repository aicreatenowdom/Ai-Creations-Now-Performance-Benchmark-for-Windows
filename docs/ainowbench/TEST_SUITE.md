# AINowBench Production Test Suite

AINowBench combines established measurement technologies with original AI Creations Now graphics and compute workloads. The complete production run generates 44 result rows. Some rows are conditional on available hardware, drivers, runtimes, or sensors.

## Graphics

Graphics scoring balances three primary performance families:

- **Spectrum Direct3D:** offscreen 720p, 1080p, 4K, and 8K rendering
- **Game-style Direct3D:** demanding 8K scene, frames-per-second measurement, and composite result
- **DirectCompute:** graphics-memory bandwidth and FP32 compute throughput

Additional diagnostic evidence can include compatible compute measurements and peak observed graphics clocks. Optional clock telemetry is informational and does not invalidate an otherwise complete result when unavailable.

## Processor

Processor scoring combines:

- Windows all-thread compression assessment
- Single-thread mathematical operations
- Gauss–Legendre calculation stages
- 7-Zip compression and decompression
- CPU-Z single-thread and multi-thread captures
- OpenSSL SHA-256 and AES-256-CBC throughput
- Stability, temperature, and available peak-clock evidence

Repeated captures and median selection are used where the published workload calls for them.

## Storage

The benchmark targets the Windows `C:` system drive and identifies its physical device only when Windows can verify the relationship. The controlled suite includes sustained read, sequential read/write, and 4 KiB random read/write measurements at multiple queue-depth profiles. The benchmark-created test file is removed after the storage stage.

## Memory

When supported by the platform, Intel Memory Latency Checker provides sustained read bandwidth, sustained non-temporal write bandwidth, and idle latency. Production 6.0 uses an adaptive workload based on safely available physical memory. Windows inventory adds installed capacity, configured speed, module count, manufacturer, and module labels.

## Publicly documented technologies

| Technology | Role |
|---|---|
| Windows WinSAT | CPU compression and sustained system-drive read |
| Microsoft DiskSpd | Controlled sequential and random storage workloads |
| Intel Memory Latency Checker | Memory bandwidth and idle latency |
| clpeak | Compatible graphics-memory and FP32 diagnostics |
| 7-Zip | Processor compression and decompression |
| CPU-Z | Processor single-thread and multi-thread benchmark |
| OpenSSL | Processor throughput measurements |
| Libre Hardware Monitor | Available processor temperature sensors |
| System Stability Tester | Calculation timing and stability evidence |
| AI Creations Now Direct3D and DirectCompute workloads | Original graphics rendering, bandwidth, and compute tests |

The installer validates its embedded production package and payload manifest before installation. See [Third-Party Notices](../../THIRD_PARTY_NOTICES.md) and the official tools page: **https://ainowbench.com/tools.html**
