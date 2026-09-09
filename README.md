# FUSE SQL Studio: Windows testing preview

**RC19 is the current download. Unsigned, non-production preview for Windows 11 x64.**

[Download RC19 browser-portable ZIP](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.19-preview/FUSE-1.0.0-rc.19-windows-x64-browser-portable-UNSIGNED-TEST-PREVIEW.zip)

[Release notes](https://github.com/anandvegaraju/FUSE-Downloads/releases/tag/v1.0.0-rc.19-preview) · [Windows 11 checklist](WINDOWS-11-TEST-CHECKLIST.md) · [Checksums](SHA256SUMS.txt)

ZIP size: 39,917,621 bytes. SHA-256: `918d50856ad26583810211b895d62715ffa547c7ce16a4fcbe7c6c3cf01eb99a`.

## What changed

- Fixed catalog object naming; default Oracle folder `/Custom/FUSE`, with a custom-folder option.
- Improved bounded recovery for small/wide result requests, including 100 rows. The original tenant failure still needs a retest.
- Bare-column suggestions insert just the column; explicit alias-dot completion stays scoped.
- Real SQL files in Documents/FUSE/Queries or a custom folder, nested imports and pinned files/folders. Originals and external edits are not overwritten.
- Optional human-reviewed MCP creation/run requests, off after each restart. Results stay in FUSE; agents receive status/counts only.
- Independence and non-production notices in Settings and the package.

Extract the whole ZIP into a new writable folder. Close the old FUSE window and console after saving, then run **Start FUSE.cmd** from RC19. Your existing RC18 workspace remains in your Windows user profile; do not delete it. Update your coding client's FUSE server entry using the new package's Settings.

This runs through a local Edge/Chrome app-style window with a default-browser fallback. It is not a native installer. No new RC19 native installer, native portable, macOS or Store package is offered here; older assets remain historical and do not contain these changes.

## Test boundary

The FUSE package is unsigned and was assembled on macOS with unchanged Windows Node runtime bytes from the previous Windows build. Local automated and synthetic UI tests passed; Windows 11, DPAPI, authorized-tenant and real coding-client acceptance for this revision remain required. It is not a signed/stable release or a way around company controls. Do not disable security protections. Ask IT if policy blocks it.

Use authorized non-production environments only. FUSE is independent software, not affiliated with, endorsed, sponsored or certified by Oracle, and grants no Oracle license. Oracle is a registered trademark of Oracle and/or its affiliates. Read the bundled legal and dependency notices.

This repository contains download documentation and preview assets, not the private application source. No telemetry or AI provider integration is added by FUSE. Your coding agent's independently granted file access and provider handling are outside FUSE's control.
