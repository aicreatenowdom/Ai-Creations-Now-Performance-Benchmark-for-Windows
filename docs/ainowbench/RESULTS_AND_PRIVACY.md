# AINowBench Results, Uploads, and Privacy

AINowBench is local-first. A complete benchmark result does not require an account or an upload.

The live privacy page is the authoritative current policy:

**https://ainowbench.com/privacy.html**

## Local files

A completed run can generate these files locally:

- PDF report
- Technical TXT report
- HTML report
- Print-ready HTML
- CSV data
- Diagnostic log
- Interface state
- Result receipt after a confirmed upload

These files remain on the computer.

## Optional online comparison

Online comparison is selected by default in AINowBench 6.0.5. The user can clear the option and confirm a local-only run before the benchmark begins.

When online comparison remains selected:

- Only the technical TXT report is transmitted over HTTPS.
- The PDF, HTML, CSV, diagnostic log, and interface state are not uploaded.
- The receiver validates the canonical result structure, measurements, scoring, points, category scores, and final tier.
- The application verifies the returned Result ID, content information, receipt, duplicate state, and comparison address.
- A local receipt is saved only after server confirmation.

## Information the technical TXT can contain

The optional technical upload is designed for validation and troubleshooting, so it contains more detail than the public result page. It can include:

- Windows computer name
- Windows user name
- Operating-system details and installation date
- Hardware inventory
- Benchmark measurements
- Local report paths
- Private Installation ID
- One-run Result ID
- Structured comparison hardware profile

## Information not written into the technical report

The public privacy documentation states that the technical report does not contain:

- IP address
- MAC address
- Disk serial number
- Email address
- Payment-card data
- Reusable login credential

Normal website, security, CDN, and download-service logs can still process ordinary request information such as IP address, date, time, requested path, browser information, and security signals.

## Public result boundary

The public comparison page is created from a sanitized allowlist. It can display:

- Overall score
- Category scores
- Tier
- Benchmark points
- Selected processor, graphics, memory, and storage labels
- Comparison ranking and related performance context

The public page does not display:

- Computer name
- Windows user name
- Local paths
- Private Installation ID
- Raw technical TXT report

## Result IDs

A Result ID is a lookup key for one server-validated run. It is not an account credential. A public Result ID is created only after the server confirms the accepted result.

Do not post a private Installation ID, raw technical report, or unredacted diagnostic log in a public GitHub issue.

## Donations

Optional donations are processed on Stripe’s hosted checkout. AI Creations Now does not intentionally collect complete payment-card numbers through the benchmark website. Donations do not unlock features or change the AINowBench installer.

## Privacy support

For a privacy question or removal request involving a submitted benchmark, use the official contact process linked from the live privacy page and include the applicable Result ID. Do not send the Windows user name or computer name unless AI Creations Now specifically requests it during a private support review.
