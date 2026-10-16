# Systems

Part of [[814 Epoxy]].

## 814 SALES DOC (Google Sheet)

- **Contract Tracker** tab: one row per job. Column A `Est #` is the job key. Column C (Phase) is filled in by people. W (QB Invoice #) and X (QB Status: Open / Partial / Paid / Void) are written by the QB status sync.
- **Dashboard** tab: A33:C34 holds the sync's reconciliation check.
- **QB AR** tab: every open invoice, oldest due date first, owned by the sync.
- The sheet's own Apps Script project runs an onEdit lead-intake trigger.

_To fill in: what the other tabs are and who uses them._

## QuickBooks Online

- Company: 814 EPOXY AND MORE.
- An invoice's DocNumber matches a Tracker row when it equals `K`, `K-D` or `K-F`, where `K` is the row's Est #.

## QB status sync

- Code and full docs: GitHub repo `fletchlivinlives/814-qb-status`.
- Standalone Google Apps Script, runs once a day. Reads invoices from QuickBooks (never writes to it) and updates W/X, Dashboard A33:C34 and the QB AR tab.
- If QuickBooks disconnects (`invalid_grant`), re-run its `authorize` steps from that repo's README.
