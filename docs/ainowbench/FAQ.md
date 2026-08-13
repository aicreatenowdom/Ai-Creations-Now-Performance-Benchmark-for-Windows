# AINowBench Frequently Asked Questions

## Is AINowBench free?

Yes. AINowBench 6.0.5 Production is a complete free desktop release. It has no subscription, trial expiration, account requirement, or feature lock. Donations are optional and do not change the software.

## Does AINowBench overclock or tune my computer?

No. It measures performance. It does not intentionally change processor or graphics clocks, voltages, firmware, or overclocking settings.

## How long does a complete run take?

Most supported systems complete in approximately 9–12 minutes. Hardware performance, drivers, virtualization, storage, optional sensors, and background activity can change the total time.

## Which Windows systems are supported?

The public requirements specify native x64 Windows with:

- A desktop environment
- Windows on `C:`
- PowerShell 5.1 components
- Administrator approval

Windows on ARM and 32-bit Windows are not supported.

## Do I need an account?

No. Downloading, installing, running locally, and browsing the public comparison database do not require an account.

## Is online comparison required?

No. Online comparison is selected by default, but it can be cleared before the run. A local-only benchmark still creates the complete local report set.

## What is uploaded?

When online comparison remains selected, AINowBench uploads the technical TXT report over HTTPS. It does not upload the PDF, HTML, CSV, diagnostic log, or interface state.

See [Results and Privacy](./RESULTS_AND_PRIVACY.md).

## What appears publicly?

The public result page can show scores, tier, points, rankings, and selected sanitized hardware labels. Computer names, user names, local paths, private Installation IDs, and the raw technical report are not displayed.

## What is a Result ID?

A Result ID is a 32-character lookup key for one server-validated run. It is not a login or account credential.

## What if a test is skipped?

A skipped capability is excluded when required hardware, runtime, driver, or sensor support is unavailable. The benchmark reports the condition rather than treating it as perfect or inventing a value.

## Why does Windows show a SmartScreen warning?

Newly published signed applications can lack enough reputation history for SmartScreen. Always verify the official source, exact SHA-256 digest, and valid Authenticode signature before running the installer.

## Where are reports saved?

The application creates a report folder under the Windows Desktop:

```text
AI Creations Performance Benchmark Reports
```

## Can I compare before-and-after upgrades?

Yes. Use the same power profile, driver strategy, background conditions, and test preparation for more meaningful comparisons.

## Is AINowBench affiliated with Microsoft, Intel, AMD, NVIDIA, 3DMark, or other benchmark vendors?

No. Product names identify hardware, tools, or comparison context. They do not imply affiliation, sponsorship, certification, or endorsement.

## How do I support development?

The download page includes an optional donation route. The same complete installer remains available without a donation:

**https://ainowbench.com/download.html**
