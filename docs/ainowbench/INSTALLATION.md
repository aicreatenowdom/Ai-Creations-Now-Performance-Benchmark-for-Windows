# Install and Run AINowBench 6.0.5

## Requirements

AINowBench 6.0.5 is designed for:

- Native 64-bit x64 Windows
- A Windows desktop environment
- Windows installed on the `C:` system drive
- Windows PowerShell 5.1 components
- Local administrator approval for installation and benchmark launch

Windows on ARM and 32-bit Windows are not supported. Organization-enforced script restrictions can prevent the benchmark from launching.

## Before downloading

Use the official download page:

**https://ainowbench.com/download.html**

The expected installer is:

```text
AiCnowBenchx64v605signed.exe
```

The expected SHA-256 digest is:

```text
B7405682DAAFF465D12C941330DCA6F5B468E06FF3074B49FD02C4E70C2F9991
```

Follow [Verify the Download](./VERIFY_DOWNLOAD.md) before running the installer.

## Prepare the computer

For a cleaner and more repeatable result:

1. Save open work.
2. Close games, renderers, virtual machines, large downloads, and demanding applications.
3. Connect laptops and mobile workstations to AC power.
4. Allow Windows Update, antivirus scans, indexing, and file synchronization to finish.
5. Use the same Windows power profile when comparing repeated runs.
6. Use stable graphics and chipset drivers when measuring representative everyday performance.

## Install

1. Open the verified installer.
2. Approve the Windows administrator prompt.
3. Follow the installation prompts.
4. AINowBench installs to:

```text
C:\AIPerfBench
```

5. Desktop and Start Menu shortcuts are created.
6. When an earlier version is detected, the installer presents an upgrade path.

## Run the benchmark

1. Open **AI Creations Now Performance Benchmark**.
2. Read the preparation notice.
3. Decide whether to use online comparison.
   - Online comparison is selected by default.
   - Clear the option and confirm the local-only notice when you do not want to submit a result.
4. Select **START BENCHMARK**.
5. Approve the Windows prompt.
6. Leave the benchmark window open until the suite finishes.

High CPU, GPU, memory, and storage utilization is expected during the relevant stages. Do not restart Windows, put the computer to sleep, disconnect AC power, or launch another demanding workload during the run.

## Review the result

A completed run shows:

- Overall score
- Performance tier
- Deterministic benchmark points
- Graphics score
- Processor score
- Storage score
- Memory score

The result folder is created under the Windows Desktop:

```text
AI Creations Performance Benchmark Reports
```

Use the application buttons to open the PDF report, technical report, results folder, and—when an upload was confirmed—the online result.

## Typical runtime

Most supported systems complete the full run in approximately **9–12 minutes**. Slower storage, processors, graphics hardware, virtualized environments, driver behavior, or unavailable optional sensors can change the total time.
