# FUSE SQL Studio: Windows testing preview

**RC20 is the current download. Unsigned, non-production preview for Windows 11 x64.**

[Download RC20 browser-portable ZIP](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.20-preview/FUSE-1.0.0-rc.20-windows-x64-browser-portable-UNSIGNED-TEST-PREVIEW.zip)

[Release notes](https://github.com/anandvegaraju/FUSE-Downloads/releases/tag/v1.0.0-rc.20-preview) · [Windows 11 checklist](WINDOWS-11-TEST-CHECKLIST.md) · [Checksums](SHA256SUMS.txt)

ZIP size: 39,924,086 bytes. SHA-256: `165e6a6550db81969ab8b96e01aa970e1669f82f0f632ae3bf39bc16e3c7cbf4`.

## What changed

- Redesigned Settings: five clear categories, consistently padded cards and aligned controls, including the lower sections.
- Three-step Coding tools setup: choose a client, copy its configuration, reconnect and try a schema-only test prompt. Windows config-file help and manual stdio fields are included.
- Separate optional action permissions, off after each restart. Every request needs approval; results stay in FUSE and agents receive status/counts only.
- Clear copy/save/error/retry feedback. Unfinished SQL-folder edits survive category navigation, with a discard action.
- All RC19 connection, SQL-file saving/import, scoped completion and bounded-fetch improvements remain included. The owner reported those core RC19 Windows workflows worked; this is not RC20 acceptance.

Extract the whole ZIP into a new writable folder. Close the old FUSE window and console after saving, then run **Start FUSE.cmd** from RC20. Your existing workspace remains in your Windows user profile; do not delete it. Update your coding client's FUSE server entry using **Settings > Coding tools**. Keep other client settings intact; copying setup alone does not verify connection.

This runs through a local Edge/Chrome app-style window with a default-browser fallback. It is not a native installer. No new RC20 native installer, native portable, macOS or Store package is offered here; older assets remain historical and do not contain these changes.

## Test boundary

The FUSE package is unsigned and was assembled on macOS with unchanged Windows Node runtime bytes from the previous Windows build. Local automated and synthetic UI tests passed; Windows 11 visual/scaling, clipboard, regression and real coding-client acceptance for this revision remain required. No Windows binary execution or fresh independent DPAPI evidence is implied by the Mac checks. It is not a signed/stable release or a way around company controls. Do not disable security protections. Ask IT if policy blocks it.

Use authorized non-production environments only. FUSE is independent software, not affiliated with, endorsed, sponsored or certified by Oracle, and grants no Oracle license. Oracle is a registered trademark of Oracle and/or its affiliates. Read the bundled legal and dependency notices.

This repository contains download documentation and preview assets, not the private application source. No telemetry or AI provider integration is added by FUSE. Your coding agent's independently granted file access and provider handling are outside FUSE's control.
