# Public Software Roadmap

This roadmap communicates direction without publishing private implementation details or promising dates that have not been approved.

## Available now

### AINowBench 6.0.5 Production

- Free native x64 Windows benchmark
- Four-category Production 6.0 scoring model
- 44 result rows across graphics, processor, storage, and memory analysis
- Detailed local PDF, TXT, CSV, HTML, and diagnostic output
- Optional server-validated comparison result and permanent receipt
- Signed installer with a published SHA-256 digest

### AUTO Deployment Production 4.7

- Guided Windows operations deployment
- Monitoring, alerts, audits, reporting, and local evidence
- Master Command Center and controlled Remote Desktop actions
- Commercial lifetime single-machine licensing for supported systems

## Planned next

### Microsoft Signing Automation

The planned public utility is intended to simplify legitimate Microsoft signing workflows for authorized users.

Proposed goals:

1. Let the user choose a supported file through Windows Explorer.
2. Detect required Microsoft and .NET prerequisites.
3. Guide authentication through the authorized Microsoft account flow.
4. Preserve the original file before attempting a signing operation.
5. Submit the file through an official Microsoft signing service available to the user.
6. Verify the completed Authenticode signature and timestamp.
7. Produce a readable log and clear success or failure result.
8. Avoid storing credentials, access tokens, or private signing material in the repository or application package.

Current distribution intent: **free software with optional donations**.

No public binary exists yet. The product name, supported file types, Microsoft service requirements, release date, and final licensing terms remain subject to production validation and approval.

## Future repository organization

As additional software becomes public, each production product should receive:

- A dedicated project page or repository
- Current signed release assets
- Release notes and version history
- Installation and verification instructions
- Privacy and security documentation
- Structured issue templates
- A clearly identified support boundary

Private source code, licensing systems, signing credentials, API secrets, receiver logic, and security-sensitive infrastructure will remain outside public repositories.
