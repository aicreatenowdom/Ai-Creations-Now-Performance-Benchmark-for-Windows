# Microsoft Signing Automation — Planned Project

AI Creations Now is planning a guided Windows utility for legitimate Microsoft code-signing workflows available only to users authorized to sign and publish the selected software.

## Current status

**Planning and documentation only.** No public executable, source package, version, release date, or final feature contract has been published.

## Intended experience

The planned utility is intended to provide:

- A normal Windows file picker for selecting software the user owns or is authorized to release
- Checks for required Microsoft and Windows development components
- Authentication through the user's authorized Microsoft account or service flow
- An original-file backup before an authorized signing operation
- Submission through an official signing service available to that account
- Authenticode signature and timestamp verification
- A readable operation log

No certificates, account credentials, tokens, or signing secrets will be bundled in the application or stored in this public repository.

## Security principles

The utility will not bypass authentication, service eligibility, Windows trust controls, or software ownership requirements. It will not sign files without the user's authorized account, store passwords in plaintext, conceal the selected file, or report success without verification.

## Distribution intent

The present intent is free Windows software supported by optional donations, with the same complete feature set regardless of donation. A future production release would include release notes, integrity hashes, verification instructions, privacy review, and fresh-computer validation.

“Microsoft Signing Automation” is a descriptive working title. Microsoft is a trademark of Microsoft Corporation. This is an independent AI Creations Now project and is not represented as a Microsoft product, partnership, certification, or endorsement.
