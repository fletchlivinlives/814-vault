# Money in

**Business:** [[814 Epoxy]]
**Trigger:** a check, card or cash payment arrives, or Joe says "got paid" / "got a deposit".
**Done when:** QuickBooks shows the payment against the right invoice, the bank deposit matches the bank statement line, and the Contract Tracker row says what happened.

The order matters: **QuickBooks first, sheet second.** The QB status sync copies QuickBooks into the Tracker every morning (W, X, QB AR, Dashboard B33). Anything typed only in the sheet never reaches the books.

## Read first

- [[Systems]] – Contract Tracker columns and the QB sync.

## Steps

### A. Payment on an invoice (job done or billed)

1. **QuickBooks → + New → Receive payment.** Customer, tick the invoice (its number is the Est #), amount, method (Check + check number), Deposit to **Payments to deposit** (QuickBooks' name for Undeposited Funds).
2. **Sheet → Contract Tracker → Phase (C) → Paid** once the invoice is paid in full. Balance Left (I) goes to 0 by itself. Leave W/X alone; the sync sets X to Paid next morning.
3. Partial payment: leave Phase as is; the sync shows X = Partial.

### B. Deposit on a job that hasn't started

1. **QuickBooks → + New → Invoice** numbered `K-D` (K = Est #), for the deposit amount, terms Due on receipt. The sync matches `K-D` to the job row.
2. **Receive payment** against that invoice, Deposit to **Payments to deposit** (QuickBooks' name for Undeposited Funds).
3. **Sheet → Contract Tracker → Deposit $ (H)** = the amount. Balance Left (I) drops by itself. Phase stays Scheduled.
4. When the job finishes, the final invoice is `K-F` for the balance.

### C. Taking checks to the bank

1. **QuickBooks → + New → Bank deposit.** Tick every payment in that trip to the bank. Total must equal the deposit slip, so it matches the one line on the bank statement.

### D. Cash

Same as A or B, method Cash. If the cash isn't going to the bank, say so; the Dashboard's "through the bank" line counts it differently.

## Needs Joe's OK

Claude can create the `K-D` deposit invoice in QuickBooks (not sent) when Joe says yes in the session. Receiving payments and bank deposits Joe does in QuickBooks; the connector can't record payments.

## Lessons

- 2026-10-16: First use: Fuller Construction $2,700 check on invoice 23953 (A), and Mental Health Assoc of Erie $22,500 deposit on 23999 (B), deposited together.
- The AutoInvoice script in the QB sync project also creates `K-D` invoices for some rows. Before making one by hand, check QuickBooks doesn't already have it.
- 2026-10-16: Deposits on jobs not started go to the **special savings** account (bank deposit there), not checking. Paid-job money goes to general checking.
- 2026-10-16: A refund from a vendor (e.g. Erie Insurance $72) is not income: categorize it to the expense it refunds.
- Deposit invoices use item Commercial Flooring (45) or Residential Flooring (40) per the job's R/I/C, matching what AutoInvoice uses.
