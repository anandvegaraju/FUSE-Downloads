# FUSE SQL Studio — Windows testing previews

**Latest app updates: RC18 browser portable · Windows 11 x64 · UNSIGNED TEST PREVIEW**

RC18 is assembled on macOS and awaits Windows 11 testing. It is not a stable, certified or Microsoft Store release. Downloads are accessible without a GitHub account; FUSE source remains private. This repository contains download information only, not FUSE source or its Git history.

## Updated download — RC18

**[Download RC18 browser-portable ZIP · 39.9 MB](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.18-preview/FUSE-1.0.0-rc.18-windows-x64-browser-portable-UNSIGNED-TEST-PREVIEW.zip)**

Extract the entire ZIP into a writable folder and double-click **Start FUSE.cmd**. The Windows runtime is included; no separate Node.js installation is needed. Keep the console open. Wait for **Workspace saved**, close the app window, then close the console.

This preview contains persistent queries/drafts/connection profiles/preferences, Windows account-bound password protection, Edge/Chrome app-window launch, FUSE branding, row caps up to 10,000, stable alphabetical schema browsing and an optional schema-only coding-agent companion. Existing lower row caps are preserved; raise both workspace and connection caps if still limited to 500.

**These new Windows behaviors await your test.** The updated app passed Mac-side automated tests, isolated workspace restart and packaged gateway/MCP checks. The bundled Windows Node runtime is unchanged from checksum-verified RC17; this does not sign FUSE or establish RC18 Windows acceptance. RC17 browser-session work already lost cannot be recovered.

[RC18 release notes](https://github.com/anandvegaraju/FUSE-Downloads/releases/tag/v1.0.0-rc.18-preview) · [Windows 11 checklist](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.18-preview/WINDOWS-11-TEST-CHECKLIST.md) · [RC18 checksum](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.18-preview/SHA256SUMS.txt)

## Older native downloads — RC17, without the RC18 updates

There is **no RC18 native installer, native portable or MSIX yet**. These separate RC17 previews remain available for older-build testing; do not use them to verify RC18 changes.

| Package | Download | Start and storage |
|---|---|---|
| RC17 native portable — no installer | [Unsigned portable ZIP · 9.8 MB](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/FUSE-1.0.0-rc.17-windows-x64-native-portable-UNSIGNED-PREVIEW.zip) | Extract the whole ZIP and open FUSE.exe. Requires Microsoft Edge WebView2 Runtime. Saves workspace in your Windows user profile and passwords in Windows Credential Manager, not beside the EXE. |
| RC17 desktop installer | [Unsigned EXE installer · 7.8 MB](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.17-preview/FUSE-1.0.0-rc.17-windows-x64-setup-UNSIGNED-PREVIEW.exe) | Current-user installation on a device that permits it. Shares the native portable's per-user workspace. |

[RC17 release, original checksums and checklist](https://github.com/anandvegaraju/FUSE-Downloads/releases/tag/v1.0.0-rc.17-preview). Its assets are unchanged. The old RC17 browser portable is session-only and lacks the persistence fixes; use RC18 for current browser-portable testing.

## Test safely

- These previews have **no trusted FUSE publisher signature**. Windows, antivirus or organization policy may warn or block them. If blocked, stop and ask the device administrator. Do not disable protections, change execution policy or install a test certificate.
- Use an authorized **Windows 11 x64** device as a standard user. No administrator elevation is intended. Other architectures/Windows versions are outside this preview's test scope.
- Back up important SQL. Browser-portable workspace data lives outside the extracted app folder in your Windows profile. SQL/profile fields are unencrypted; do not embed secrets in SQL. DPAPI passwords are account-bound and are not transferable between PCs. Native storage is separate. Portable does not mean no local data is left behind.
- Schema browsing, suggestions and documentation links need no Oracle connection. Connected testing needs authorized **non-production** Oracle Fusion access. Save & prepare can create missing preset FUSE XDM/XDO objects in the configured existing BI Publisher folder; obtain the environment owner's permission first.
- The optional MCP companion exposes schema metadata and reviewed joins, not connections, credentials, SQL drafts, result rows or query execution. Independently granting an agent filesystem access or uploading sensitive material is outside this boundary.
- Report **Pass / Fail / Blocked / Not tested**, your Windows/browser version and redacted errors. Do not share passwords, tenant URLs, sensitive SQL, result rows or raw logs.

## Exact-build provenance

RC18 application source: a53c7f573d2add3dbbb26d2e010b9ec62b88afe0. ZIP SHA-256: cd2aaaf50b8b0ec01505db32e6dc88ab6cfcce122cce8907c5f703db730feaa6. A matching checksum confirms integrity, not publisher trust. RC18 Windows startup, real DPAPI save/restart and live coding-client acceptance remain pending.

The owner authorized these narrowly labelled Windows testing previews. This is not completed third-party rights review, stable-release approval or Store submission approval. No macOS package, MSIX, test certificate, private evidence archive or owner workspace is published here. Automatic GitHub “Source code” archives contain this download repository's documents, not the FUSE application source. File sizes use decimal MB.
