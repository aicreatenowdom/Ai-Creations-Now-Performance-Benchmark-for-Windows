# AINowBench 6.0.5 Production

<p align="center">
  <img src="../../assets/ainowbench-product-card.svg" alt="AINowBench 6.0.5 Production" width="100%">
</p>

AINowBench is a free Windows desktop benchmark developed by AI Creations Now Software Development. It measures graphics, processor, storage, and memory performance, generates detailed local reports, and can optionally submit a sanitized result profile to the public comparison database after server validation.

## Quick links

- [Download the signed installer](https://ainowbench.com/download.html)
- [Official product website](https://ainowbench.com/)
- [Installation guide](./INSTALLATION.md)
- [Verify the download](./VERIFY_DOWNLOAD.md)
- [Scoring methodology](./SCORING.md)
- [Test suite](./TEST_SUITE.md)
- [Results and privacy](./RESULTS_AND_PRIVACY.md)
- [Troubleshooting](./TROUBLESHOOTING.md)
- [Frequently asked questions](./FAQ.md)
- [6.0.5 release notes](./RELEASE_6.0.5.md)

## Current release

| Field | Value |
|---|---|
| Product | AI Creations Now Performance Benchmark / AINowBench |
| Version | 6.0.5 Production |
| Scoring generation | Production 6.0 |
| Platform | Native x64 Windows desktop |
| Distribution | Signed single-file EXE |
| License model | Free desktop edition; optional donations |
| Account required | No |
| Online comparison | Optional; selected by default and can be cleared before the run |
| Typical runtime | Approximately 9–12 minutes, depending on system performance |
| Installer filename | `AiCnowBenchx64v605signed.exe` |
| SHA-256 | `B7405682DAAFF465D12C941330DCA6F5B468E06FF3074B49FD02C4E70C2F9991` |

## What the benchmark measures

AINowBench produces a complete score from four weighted categories.

| Category | Weight | Primary evidence |
|---|---:|---|
| Graphics | 41.18% | Direct3D rendering, DirectCompute, game-style rendering, GPU bandwidth, and compute evidence |
| Processor | 29.41% | Windows assessment, mathematical workloads, 7-Zip, CPU-Z, OpenSSL, and stability evidence |
| Storage | 17.65% | Sustained, sequential, and random C: system-drive performance |
| Memory | 11.76% | Sustained read/write bandwidth, idle latency, and installed-memory inventory |

<p align="center">
  <img src="../../assets/ainowbench-score-model.svg" alt="AINowBench Production 6.0 scoring model" width="100%">
</p>

## What you receive

A completed run can create:

- A polished PDF report
- A detailed technical TXT report
- Supporting HTML and print-ready HTML
- CSV hardware and result data
- Diagnostic evidence and logs
- A local result folder on the Windows Desktop
- An optional validated Result ID and permanent online receipt

The reports remain on the computer whether or not online comparison is used.

## Local-first workflow

<p align="center">
  <img src="../../assets/ainowbench-workflow.svg" alt="AINowBench workflow" width="100%">
</p>

1. Download from the official website.
2. Verify the SHA-256 digest and Windows Authenticode signature.
3. Close demanding applications and connect laptops to AC power.
4. Run the guided benchmark without interruption.
5. Review the local reports.
6. Optionally use the server-validated comparison system.

## Transparency

The scoring model is fixed and deterministic. Measurements are normalized against defined curves, related results are consolidated into performance families, and the four category scores are combined with the published 7:5:3:2 weighting.

Unavailable capabilities are not silently treated as perfect results. Supported outcomes are reported honestly, including skipped, review, diagnostic, partial-telemetry, and unavailable conditions.

## Independent project notice

AINowBench is an independent AI Creations Now engineering project. References to Microsoft, Intel, AMD, NVIDIA, CPUID, 7-Zip, OpenSSL, DiskSpd, Intel MLC, clpeak, Libre Hardware Monitor, System Stability Tester, Futuremark, UL Solutions, 3DMark, or other products identify technologies or comparison context only. They do not imply affiliation, sponsorship, certification, or endorsement.
