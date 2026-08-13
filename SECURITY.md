# Security Policy

AI Creations Now treats software authenticity, user privacy, and responsible vulnerability handling as important parts of every public release.

## Private reporting

Do not publish security-sensitive information in a GitHub issue, discussion, screenshot, or attached log. Contact AI Creations Now privately through the official company website:

**https://aicreatenow.com/**

Toll-free: **1-866-315-4750**

Include the affected product and version, a concise description, the date observed, and a safe way to reproduce the behavior. Remove personal information and customer data before sending supporting material.

## Official sources

Treat software as official only when it comes from:

- `https://aicreatenow.com/`
- `https://ainowbench.com/`
- `https://ainowbench.com/download.html`
- This GitHub account and its published release assets

Do not rely on unofficial mirrors, unsolicited attachments, shortened links, or files redistributed by unknown third parties.

## Verify before execution

For every public installer:

1. Confirm the product name, version, and filename.
2. Calculate the SHA-256 digest.
3. Compare it with the value published by AI Creations Now.
4. Inspect the Windows Authenticode signature and timestamp.
5. Stop when any value differs.

AINowBench instructions are available in [Verify AINowBench 6.0.5](./docs/ainowbench/VERIFY_DOWNLOAD.md).

## Public repository boundary

This repository contains public documentation, branding, policies, issue forms, release information, and approved public assets. Private account material, customer information, production service configuration, and unpublished implementation details are intentionally excluded.
