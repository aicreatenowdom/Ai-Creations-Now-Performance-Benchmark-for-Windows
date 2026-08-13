# AINowBench Troubleshooting

## Windows displays a SmartScreen or reputation warning

AINowBench is a recently published Windows application. Microsoft SmartScreen can display a reputation warning even when a file is correctly signed.

Before making any decision:

1. Confirm the installer came from `https://ainowbench.com/download.html`.
2. Verify the exact SHA-256 digest.
3. Confirm that Windows reports a valid Authenticode signature.
4. Stop if the hash or signature does not match.

See [Verify the Download](./VERIFY_DOWNLOAD.md).

## The installer hash does not match

Do not run the file.

- Delete the copy.
- Download it again from the official page.
- Recalculate the SHA-256 digest.
- Do not use a third-party mirror.

The 6.0.5 expected digest is:

```text
B7405682DAAFF465D12C941330DCA6F5B468E06FF3074B49FD02C4E70C2F9991
```

## A GPU or compute test is skipped

A skipped test does not automatically mean the computer failed.

Possible reasons include:

- Unsupported or unavailable graphics runtime
- Integrated or virtual graphics limitations
- Driver capability
- Missing optional OpenCL, CUDA, or Vulkan exposure
- Remote or virtual environment restrictions
- Hardware identity not sufficiently verified

Review the technical report for the row-specific explanation. Update to a stable graphics driver when appropriate and run again under the same conditions.

## Processor temperature is unavailable

Processor-temperature evidence depends on supported sensor access. Some virtual machines, firmware configurations, processor platforms, security policies, or drivers do not expose a compatible sensor.

Production 6.0 can report the thermal measurement as unavailable while preserving the rest of the benchmark, reports, scoring, and optional upload.

## The benchmark takes longer than expected

The typical full run is approximately 9–12 minutes, not a guaranteed limit. Total time can vary because of:

- Slower CPU, GPU, memory, or storage
- Virtualization
- Background activity
- Driver initialization
- Optional runtime discovery
- Storage latency
- Sensor timeouts and bounded recovery
- A very slow mathematical stage

Keep the live benchmark window open unless the application clearly reports a terminal error.

## An online result did not upload

The complete local result remains available.

Production 6.0 includes:

- Three immediate upload attempts when needed
- An automatic retry queue for recoverable interruptions
- Manual **Retry Upload**
- A separate completed-result recovery route
- Response and verification logging

Do not repeat the entire benchmark immediately if the completed local result can be submitted through the retry or recovery workflow.

## No Result ID was created

A Result ID appears only after server confirmation. Common explanations include:

- The run was intentionally local-only.
- The upload is still pending or retrying.
- The server rejected an incomplete or invalid result.
- Network or receiver verification did not complete.

Review the local receipt and technical logs before opening an issue.

## Report files are missing

Confirm that the benchmark reached its completion screen. Reports are normally created under:

```text
Desktop\AI Creations Performance Benchmark Reports
```

Search the Desktop and review the diagnostic log. Do not publicly post an unredacted technical TXT or diagnostic log.

## Opening a GitHub issue

Use the structured issue form and include:

- AINowBench version
- Windows edition and build
- Processor
- Graphics adapter
- Memory capacity
- System-drive type
- Exact stage or row
- What you expected
- What actually happened
- Reproduction steps

Remove computer names, Windows user names, local paths, credentials, private IDs, email addresses, and other personal information.
