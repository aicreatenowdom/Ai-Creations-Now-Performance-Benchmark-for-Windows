# Verify the AINowBench 6.0.5 Download

These checks are for verifying the official AINowBench installer that you downloaded for your own computer. Do not rely on the filename alone. Verify both the published SHA-256 digest and the Windows Authenticode signature before running the installer.

## Official release values

| Field | Expected value |
|---|---|
| Filename | `AiCnowBenchx64v605signed.exe` |
| Version | 6.0.5 Production |
| SHA-256 | `B7405682DAAFF465D12C941330DCA6F5B468E06FF3074B49FD02C4E70C2F9991` |
| Official download page | `https://ainowbench.com/download.html` |
| GitHub release tag | `ReleaseV60` |

A plain checksum record is also available in [`SHA256SUMS.txt`](./SHA256SUMS.txt).

## PowerShell verification

Open Windows PowerShell and run:

```powershell
$file = "$env:USERPROFILE\Downloads\AiCnowBenchx64v605signed.exe"

Get-FileHash -Path $file -Algorithm SHA256
Get-AuthenticodeSignature -FilePath $file |
    Format-List Status, StatusMessage, SignerCertificate, TimeStamperCertificate
```

The hash must exactly match:

```text
B7405682DAAFF465D12C941330DCA6F5B468E06FF3074B49FD02C4E70C2F9991
```

The Authenticode status should report `Valid`. Inspect the signer and timestamp information shown by Windows before proceeding.

## Command Prompt alternative

```bat
certutil -hashfile "%USERPROFILE%\Downloads\AiCnowBenchx64v605signed.exe" SHA256
```

Compare the returned digest character for character with the published value.

## Windows graphical signature check

1. Right-click the installer.
2. Select **Properties**.
3. Open the **Digital Signatures** tab.
4. Select the listed signature.
5. Select **Details**.
6. Confirm that Windows reports the digital signature as valid.
7. Review the signer and timestamp details.

## Stop when any verification fails

Do not run the file when:

- The hash differs by even one character.
- The Digital Signatures tab is missing when a signed installer is expected.
- Windows reports an invalid, corrupted, or untrusted signature.
- The file came from an unofficial mirror, unsolicited message, or unknown third party.
- The filename or version does not match the release being documented.

Delete the unverified copy and download it again from the official AINowBench page.

## SmartScreen notice

A correctly signed new application can still receive a Microsoft SmartScreen reputation warning. A reputation warning is not a substitute for verification. Confirm the official source, exact hash, and valid Authenticode signature before deciding whether to continue.
