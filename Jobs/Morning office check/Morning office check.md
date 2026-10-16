# Morning office check

**Business:** [[814 Epoxy]]
**Trigger:** scheduled task "814 morning office check", weekdays 6:52am Eastern (result goes to Joe by push notification and email), or Joe says "morning check". The scheduled task needs the Intuit QuickBooks and Google Drive connectors attached in claude.ai.
**Done when:** Joe has one short message listing what needs him today, and today's daily note has a line saying the check ran.

This job only reads. It never sends anything to a customer, never edits the SALES DOC and never writes to QuickBooks.

## Read first

- [[Systems]] – the SALES DOC tabs and QuickBooks.
- [[People]] – who the crew leads are.

## Steps

1. **Money owed (QuickBooks, live).** Run the A/R Aging Summary as of today. List every customer with an overdue balance: name, amount, aging bucket. Give total receivables, current and overdue. Use QuickBooks, not the QB AR tab, because the tab is only as fresh as the last nightly sync.
2. **Leads going cold (SALES DOC → Dashboard).** Read the NEEDS ATTENTION block at the top of the Dashboard tab: overdue follow-ups, due in the next 7 days, BID OUT with no next action, SCOUTED never priced. Give each count and value.
3. **This week and next (SALES DOC → SCHEDULE_FEED).** List the jobs active or starting in the next 14 days with dates and crew lead. Flag any job with no crew lead.
4. **Gaps (SALES DOC → FEED).** Count won estimates marked "⚠ NOT IN TRACKER". A phased job tracked as `K-1`, `K-2`… (like West Ridge 23916) gets flagged even though it's tracked; say so instead of counting it as a gap.
5. **Write the message.** It reads on a phone in under a minute:
   - first line: the one thing that most needs Joe today
   - then up to 3 short sections: **Money**, **Leads**, **Schedule**; skip a section if nothing in it needs action
   - plain numbers; no tables
6. **Log it.** Add one line to today's daily note under a "Morning office check" section with the headline numbers. Commit and push. If the push is refused (403), don't retry: put one line at the end of the message saying the log didn't save. The message to Joe matters more than the log.

## Needs Joe's OK

Nothing in this job sends or changes anything. If the check suggests a follow-up (a payment reminder, a call), list it as a suggestion; never send it.

## Lessons

- 2026-10-16: The Google Drive connector returns only the first rows of each tab. That covers the Dashboard's NEEDS ATTENTION block, SCHEDULE_FEED and the top of FEED, but not full scans of Customer Leads or the Contract Tracker. Don't present a partial scan as complete.
- 2026-10-16: First run by hand. QuickBooks showed $59,856.50 receivable, $6,740.00 overdue (Fuller Construction $2,700 and Paterniti Winston and Angela $4,040, both 1–30 days). The Dashboard showed 48 overdue lead follow-ups worth $352,285.
- 2026-10-16: First scheduled test run worked: QuickBooks and Drive read fine, push notification sent. Pushing the log to the vault failed (403) because the scheduled task had no GitHub repo attached; Joe adds `814-vault` to the scheduled task's repositories to fix it.
