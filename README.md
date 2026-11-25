# JMK Voter List

## Files to upload to GitHub

Upload/replace these two files in the root of your existing repository:

- `index.html` — updated voter app page with Google Sheets Party read/save support.
- `README.md` — this setup guide.

**Keep your existing `voter-data.js` file. Do not delete or replace it.** The app needs it to display the voter records.

## Google Apps Script

The Apps Script attached to your Google Sheet should use the updated `doGet(e)` code that was just deployed. The sheet tab name must be exactly `Voter Details`, with:

- Column A: `S.No`
- Column B: `Party`

The Web App URL is already configured in `index.html`.

## GitHub upload

1. Open your existing `JMK-Voter-List` repository.
2. Upload/replace `index.html` and `README.md` in the repository root.
3. Commit the changes.
4. Wait a minute, then open: https://haribabu2bi-stack.github.io/JMK-Voter-List/

## Test

1. Open the app.
2. Wait until the status says `Party data connected to Google Sheets.`
3. Enter a Party value for a test S.No and click Save.
4. Confirm that the same S.No row in the `Voter Details` sheet has the Party value in column B.
5. Refresh the app and confirm the Party value remains visible.

If the app says it cannot connect, check that the Apps Script Web App deployment is accessible to users with the intended access setting.
