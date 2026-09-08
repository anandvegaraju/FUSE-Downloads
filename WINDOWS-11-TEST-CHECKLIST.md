# RC18 browser portable — Windows 11 test checklist

UNSIGNED TEST PREVIEW. Assembled on macOS from a53c7f573d2add3dbbb26d2e010b9ec62b88afe0; the FUSE application has not yet been run on Windows for this revision. The Windows runtime is byte-for-byte from verified RC17. This is not a new native installer, Store package or stable release.

1. Extract the whole ZIP into a writable folder (include a space in its name). Double-click Start FUSE.cmd. Expect an Edge/Chrome app window with FUSE branding, no usual tab strip and no administrator prompt. If policy blocks it, report Blocked; do not disable security controls.
2. Create a test connection, saved query and unsaved draft. Wait for Workspace saved. Close the window, then console. Relaunch: profiles, SQL and preferences must remain. Check that the saved password works after restart under the same Windows account. FUSE should never ask you to change PowerShell execution policy.
3. Copy the application folder elsewhere and launch the new copy under the same Windows account. Your workspace should remain available. A second simultaneous console must fail clearly, not overwrite it.
4. Set workspace and connection caps above 500. Run a permitted query requesting 1,000 rows; check the count, export and cancellation. Keep evidence synthetic or redacted, not tenant data.
5. Schema: confirm A-Z order stays unchanged when clicking/favoriting tables; PAPF has 105 column comments. SQL: SELECT PAPF. FROM PER_ALL_PEOPLE_F PAPF — place the cursor after the dot and check alias-specific suggestions. Open an official documentation link.
6. Settings > External coding agents: copy the setup into a separate coding-client project. Close FUSE and confirm schema lookup still works. Check exactly five schema-only tools, PAPF columns and a person-to-absence join. There must be no query-execution, connection, credentials, history or arbitrary-file tool.
7. Copy schema for agent / Copy reviewed context should include metadata and citations, not your SQL or results. Do not independently grant your agent access to the FUSE workspace folder.

Reply with Windows build, Edge/Chrome version, package SHA-256 and Pass / Fail / Blocked / Not tested for each item. Share redacted error text only; no passwords, tenant URLs, usernames, real SQL literals or result rows. Do not call a skipped check a pass.
