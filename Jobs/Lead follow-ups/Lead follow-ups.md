# Lead follow-ups

**Business:** [[814 Epoxy]]
**Trigger:** Joe says "follow-ups", or the [[Morning office check]] shows overdue follow-ups.
**Done when:** every overdue BID OUT lead has either a follow-up draft waiting in Gmail for Joe, or a note from Joe on why not (dead, waiting on budget, already talked).

## Read first

- [[Systems]] – the Customer Leads tab and the Dashboard.
- [[Customer categories]] – nonprofits and public bodies buy on budgets and boards; follow up on their timeline, not a homeowner's.

## Steps

1. **Pull the list.** Export the 814 SALES DOC as .xlsx with the Drive connector (`download_file_content`, export type xlsx); the plain read only shows the first rows. Overdue = Next Action Date before today and Status not WON or LOST (the Dashboard's rule).
2. **Money first.** Work BID OUT rows by Bid $, largest first. Other statuses (NEW / INTAKE, REWORK, ALTERNATE, COLD) come after, in a separate pass.
3. **Check before drafting.** Search Gmail for the customer's email address and company. If they replied or Joe wrote to them after the Next Action Date, don't draft; tell Joe what the latest thread says.
4. **Ask Joe one line per lead** when the sheet doesn't say enough: still alive? anything said by phone? He answers in a batch.
5. **Draft, don't send.** Create a Gmail draft per lead (email on file), short, in Joe's voice: reference the job, the price sent and one easy next step. Phone-only leads get a call reminder instead, with the number and a one-line script.
6. **Report.** One list: drafted, call reminders, skipped with reason. Suggest the new Next Action and date for each row; Joe updates the sheet (or approves Claude doing it once sheet edits are allowed).

## Needs Joe's OK

Every email. Drafts sit in Gmail until Joe sends them himself.

## Lessons

- 2026-10-16: First pull: 49 overdue rows, $352,285.02 bid. All the money is in 19 BID OUT rows; TitanX ($181,220) is half of it. 29 have email, 17 phone only, 3 neither.
- 2026-10-16: The Dashboard misses BID OUT rows with no Next Action Date (Fuller $3,000, Arkelian $3,500, row 205 $20,000 with no company). Include them in step 2.
- 2026-10-16: Date Sent is blank on most BID OUT rows, so "how long since we sent the price" has to come from Gmail.
