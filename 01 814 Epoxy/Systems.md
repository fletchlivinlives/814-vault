# Systems

Part of [[814 Epoxy]].

## 814 SALES DOC (Google Sheet)

Where Joe estimates, contracts and schedules. Still being built out. Its own **How This Works** tab explains it: Leads feed the Tracker, the Dashboard reads both.

- **Customer Leads** tab: every opportunity, one row per bid. Status, job status, source, R/I/C, next action and date, estimate # and bid $. The header shows the next estimate number.
- **FEED** tab: won estimate numbers, flagged "⚠ NOT IN TRACKER" when they have no Tracker row.
- **SCHEDULE_FEED** tab: jobs by week with dates, crew lead and weekly totals.
- **AUTO-INVOICE STATE / AUTO-INVOICE LOG** tabs: an auto-invoicing script, tested in Oct 2026 (dry runs on a copy, then a test invoice). Status and rules: _to fill in_.
- **Vcita Contracts / Vcita Clients** tabs: history imported from Vcita, the older system (estimates back to 2024, about 700 clients).
- **Contract Tracker** tab: one row per job. Column A `Est #` is the job key. Column C (Phase) is filled in by people. W (QB Invoice #) and X (QB Status: Open / Partial / Paid / Void) are written by the QB status sync.
- **Dashboard** tab: the NEEDS ATTENTION block at the top (overdue follow-ups, due in 7 days, bids with no next action, scouted but never priced). A33:C34 holds the QB sync's reconciliation check.
- **QB AR** tab: every open invoice, oldest due date first, owned by the sync.
- The sheet's own Apps Script project runs an onEdit lead-intake trigger.

_To fill in: how estimating, contracts and scheduling work day to day in these tabs._

## QuickBooks Online

- Company: 814 EPOXY AND MORE. Bookkeeping is being taken over from the former bookkeeper; expect cleanup.
- Customer types are Commercial / Residential / Industrial today; see [[Customer categories]].
- An invoice's DocNumber matches a Tracker row when it equals `K`, `K-D` or `K-F`, where `K` is the row's Est #.

## QB status sync

- Code and full docs: GitHub repo `fletchlivinlives/814-qb-status`.
- Standalone Google Apps Script, runs once a day. Reads invoices from QuickBooks (never writes to it) and updates W/X, Dashboard A33:C34 and the QB AR tab.
- If QuickBooks disconnects (`invalid_grant`), re-run its `authorize` steps from that repo's README.
- Updating it is manual, in the **814 QB Status Sync** project at script.google.com (not the AutoTrackerRow project bound to the sheet). The live project also has AutoInvoice.gs and Reconcile.gs that the repo doesn't, so make targeted edits rather than replacing whole files. Failures email Joe ("Summary of failures for Google Apps Script: 814 QB Status Sync").

## Other tools and services

- **Engage** – website.
- **Flory** – online floor presentations for customers.
- **ClockShark** – crew clock-in and clock-out for payroll; Rob reviews it Mondays.
- **ECAA** – payroll; **SKM** – taxes. See [[People]].
