# FUSE SQL Studio — Windows preview

**RC17 · Windows 11 x64 · Free testing preview · UNSIGNED**

Try the existing RC17 Windows build and help check the developer experience. This is an evaluation preview, not a stable release or a Microsoft Store-certified download. These downloads are publicly accessible without a GitHub account; the FUSE source repository remains private. This repository contains download information only, not the application source or its Git history.

## Choose your download

| Package | Download | Start and storage |
|---|---|---|
| **Native portable — no installer** | [Download unsigned portable ZIP · 9.8 MB](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/FUSE-1.0.0-rc.17-windows-x64-native-portable-UNSIGNED-PREVIEW.zip) | Extract the entire ZIP to a writable folder; open `FUSE.exe`. Requires Microsoft Edge WebView2 Runtime. Saves the workspace in your Windows user profile and passwords in Windows Credential Manager, **not beside the EXE**. |
| **Desktop installer** | [Download unsigned EXE installer · 7.8 MB](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/FUSE-1.0.0-rc.17-windows-x64-setup-UNSIGNED-PREVIEW.exe) | Current-user installation. Run the setup file on a device that permits it. Native portable and installer share the same per-user workspace; they are not isolated test accounts. |
| Optional browser portable — session only | [Download unsigned browser portable ZIP · 40.8 MB](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/FUSE-1.0.0-rc.17-windows-x64-browser-portable-UNSIGNED-PREVIEW.zip) | Extract the entire ZIP and open `Start FUSE.cmd`. Keep its console open. Uses your browser and a bundled runtime; no global Node.js installation is needed. Closing the console clears connection profiles, credentials and workspace state. Explicitly exported files remain. |

File sizes use decimal MB. Choose the native portable first if you do not want to install FUSE. The browser portable is a separate session-only option, not a way around blocked native execution. In GitHub's Assets list, choose the named Windows files above; the automatic “Source code” ZIP/tar.gz contains only this download repository's documents.

## Before you launch

- FUSE has **no trusted publisher signature** in this preview. Windows, antivirus or an organization policy may warn or block it. If blocked, stop and request approval from the device administrator; do not disable protections, alter execution policy or install a test certificate.
- Test on an authorized **Windows 11 x64** device as a standard user. Other architectures and older Windows versions are outside this preview's test scope. If a runtime is missing or setup asks for elevation, record that and stop; do not change the device's security configuration.
- Schema browsing, column suggestions and documentation links can be tested without an Oracle connection. Connected testing needs your own authorized **non-production** Oracle Fusion access. “Save & prepare” can create missing preset FUSE XDM/XDO objects in the configured existing BI Publisher folder; get the environment owner's permission first.
- Back up important SQL before testing. Portable does not mean the native app leaves no local data. Installer removal must not be assumed to erase the shared workspace or credentials.

## Test and report

Follow the [short Windows 11 checklist](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/WINDOWS-11-TEST-CHECKLIST.md). Return pass/fail/blocked results to the person who shared this preview. Do not share passwords, tenant URLs, personal or business data, sensitive SQL, or raw logs.

The RC17 hosted checks passed native launch, Windows credential-vault operations and installer install/launch/uninstall on Windows Server 2022. Automated tests also passed. **A clean Windows 11 client and your authorized Oracle environment have not yet been accepted**—that is the purpose of this preview. No Store certification or public Store submission is claimed.

## Exact-build provenance

These are the unchanged RC17 package bytes, with clearer outer filenames. Compare downloaded SHA-256 values with [SHA256SUMS.txt](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/SHA256SUMS.txt), for example in PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\FUSE-1.0.0-rc.17-windows-x64-native-portable-UNSIGNED-PREVIEW.zip'
```

A matching checksum confirms file integrity, not publisher trust or safety. RC17 is built from application source commit `25a60e6d3db816adcac67b7a1eda28803ee54cee`; this download repository's tag identifies its accompanying documents, not application source. Windows may display the underlying application version as `1.0.0`.

Earlier private-candidate notices remain inside the unchanged ZIPs. The owner subsequently authorized this Windows RC17 evaluation preview on 6 September 2026. That does not represent completed third-party rights review, signing, general-release acceptance, or Microsoft Store approval. No macOS package, MSIX, development certificate, private evidence archive or owner workspace is included here.
