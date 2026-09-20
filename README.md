# FUSE SQL Studio: Windows testing preview

**RC21 is the current download. Unsigned, non-production preview for Windows 11 x64.**

[Download RC21 browser-portable ZIP](https://github.com/anandvegaraju/FUSE-Downloads/releases/download/v1.0.0-rc.21-preview/FUSE-1.0.0-rc.21-windows-x64-browser-portable-UNSIGNED-TEST-PREVIEW.zip)

[Release notes](https://github.com/anandvegaraju/FUSE-Downloads/releases/tag/v1.0.0-rc.21-preview) · [Windows 11 checklist](WINDOWS-11-TEST-CHECKLIST.md) · [Checksums](SHA256SUMS.txt)

ZIP size: 39,926,649 bytes. SHA-256: `0e342b1326b4849c04c27f586587ca28cfe487922629569db1545aff173a288f`.

## What changed

- Query toolbar actions remain reachable in narrower windows, including Format, Save as and the row safety cap.
- Schema details have full primary keys, readable narrow-window columns, sticky column search and sensible detail scrolling without reordering the table list.
- Relationship paths, join explanations, source links and SQL previews are more readable through the lower sections.
- Settings retains five clear categories and consistent cards; category changes start at the top while unfinished SQL-folder edits survive.
- The library has a collapsible SQL import section, clearer empty/search states and keyboard-visible menus. Dialogs and the command palette have improved readability and navigation.
- MCP setup remains guided and optional. Fresh setup fixes canonical bridge paths; error dismissal does not retry an action. Creation/execution start off and every request needs approval. Results stay in FUSE; agents receive status/counts only.
- RC19 connection, file saving/import, persistence and completion improvements remain included. The owner's core RC19 Windows acceptance is not automatically RC21 acceptance.

Extract the whole ZIP into a new writable folder. Close the old FUSE window and console after saving, then run **Start FUSE.cmd** from RC21. Your existing workspace remains in your Windows user profile; do not delete it. Update your coding client's FUSE server entry using **Settings > Coding tools**. Keep other client settings intact; copying setup alone does not verify connection.

This runs through a local Edge/Chrome app-style window with a default-browser fallback. It is not a native installer. No new RC21 native installer, native portable, macOS or Store package is offered here; older assets remain historical and do not contain these changes.

## Test boundary

The FUSE package is unsigned and was assembled on macOS with unchanged Windows Node runtime bytes from the previous Windows build. Local checks passed: 242 JavaScript tests, 67 Rust library tests, the end-to-end UI flow, packaged gateway/schema/optional-request checks and full npm dependency audit (zero vulnerabilities). One actual-Windows-DPAPI test was skipped on Mac; Windows 11 visual/scaling, clipboard, regression and real coding-client acceptance for this revision remain required. No Windows binary execution or fresh independent DPAPI evidence is implied by the Mac checks. It is not a signed/stable release or a way around company controls. Do not disable security protections. Ask IT if policy blocks it.

Use authorized non-production environments only. FUSE is independent software, not affiliated with, endorsed, sponsored or certified by Oracle, and grants no Oracle license. Oracle is a registered trademark of Oracle and/or its affiliates. Read the bundled legal and dependency notices.

This repository contains download documentation and preview assets, not the private application source. No telemetry or AI provider integration is added by FUSE. Your coding agent's independently granted file access and provider handling are outside FUSE's control.
