# FUSE RC17 — short Windows 11 test checklist

**Unsigned evaluation preview · Windows 11 x64 · Standard user**

Use an authorized test device. If Windows or company policy blocks the app, record **Blocked** and stop; do not bypass protections. Native portable needs WebView2. Back up important SQL, extract ZIPs fully, and test one package at a time.

1. **Launch and feel:** Open the native portable's `FUSE.exe` without installing FUSE. Resize the window and switch Editor, Schema and Relationships. Check readable text, clickable controls and responsive scrolling. Note delays, freezes or unexpected elevation requests.
2. **Alias-specific suggestions:** Enter the SQL below. Move the cursor immediately after `PAPF`, type a dot, and check the dropdown appears automatically with columns such as `PERSON_ID` and `PERSON_NUMBER` from `PER_ALL_PEOPLE_F`. Type `PER` to filter and use arrows/Enter to insert. Suggestions must not switch to unrelated tables. No query execution is needed.

   ```sql
   SELECT PAPF
   FROM PER_ALL_PEOPLE_F PAPF
   ```

3. **Schema and links:** Search `PER_ALL_PEOPLE_F`, `ANC_PER_ABS_ENTRIES`, and a Finance/Common object you know. Check column descriptions and keys, and click **Open official documentation**: it should open the matching Oracle page in your browser. RC17 has published comments for all 105 People and 215 absence-entry columns; some views genuinely lack published column comments, so report the exact object/column and documentation link when a detail seems missing. Inspect one familiar relationship without assuming every suggested join fits your business case.
4. **Optional authorized connection/query:** Only with permission for a non-production tenant and any missing preset BI Publisher objects, save/prepare a connection. Run `SELECT 1 FROM DUAL`, then a small approved query. Check row limits, scrolling and CSV/XLSX/JSON exports using non-sensitive data. Try invalid SQL and cancel a running request; the UI should recover without hanging. Cancelling FUSE's wait is not a guarantee that Oracle cancels its server-side job.
5. **Persistence and safe actions:** Save a harmless draft, quit normally and reopen the native app. Verify the draft and saved connection work without exposing the password. Cancel a removal dialog with Escape and confirm the item remains; delete only a disposable test item. No tenant access? Mark connection checks **Not tested**, not passed.
6. **Installer lifecycle:** Close the portable, run the EXE setup as a standard user, launch it from Windows, then uninstall through Settings > Apps. Record launch/uninstall errors. Portable and installer share per-user data: uninstall does not imply the workspace or credentials were erased. Do not delete an existing workspace to test cleanup.
7. **Optional browser portable:** Extract separately, open `Start FUSE.cmd`, and repeat a quick schema/dropdown check. Close its console, restart, and confirm disposable drafts/connections are gone. Exported files remain. A policy block means stop, not try this as a bypass.

## Send back a short result

- Windows 11 version/build and x64 device:
- Package filename (RC17):
- Checks 1–7: Pass / Fail / Blocked / Not tested:
- Issue: steps, expected result, actual result, approximate delay:
- Redacted screenshot if useful:

Send feedback privately to the person who shared FUSE. Do not include passwords, tenant URLs, personal/business data, sensitive SQL or raw logs. Clean Windows 11 and connected acceptance remain pending until these results are reviewed.
