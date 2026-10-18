# Bookkeeping

Part of [[814 Epoxy]]. Joe keeps the books with Claude (no outside bookkeeper; SKM agreed, 2026-10-17). QuickBooks setup and accounts are in [[Systems]]; recording money in is [[Money in]].

## Source of truth for categories

Joe's sheet **"Exported Transactions ALL OF 2026 814 EPOXY"** (Google Drive) holds the 2026 bank export sorted into one tab per category, with a 24-row merchant keyword map on the SUMMARIES tab (keyword → merchant → bucket). It is the rulebook for QuickBooks categories and bank rules.

## Tab → QuickBooks account (proposed; Joe to confirm)

| Joe's tab | 2026 total (to ~10/10) | QuickBooks account |
|---|---|---|
| Raw Mat | -93,917.64 | Cost of goods sold:Material |
| Payroll | -93,847.79 | mostly **transfers** to the payroll share account (see problems) |
| Draws | -63,393.43 | Partner Distributions – Joe (or the partner whose draw it is) |
| Vehicles | -32,048.14 | Auto:Vehicle gas & fuel / repairs |
| Facilit | -19,736.43 | Utilities / facility costs |
| Rent | -17,677.00 | Rent |
| Tooling | -11,950.58 | Tools |
| Insur | -11,564.79 | Insurance |
| Soft | -8,235.85 | Office expenses:Software & apps |
| Shop Supp | -6,701.64 | Supplies |
| Meals | -5,822.21 | Meals |
| TaxesFees | -5,490.57 | Taxes & licenses / bank fees |
| MachEqip | -3,433.69 | Equipment (large items may be assets: ask SKM) |
| Cloth | -2,793.07 | Uniforms / work clothing |
| Job Site Costs | -1,769.80 | Job supplies / dumpster |
| Adv | -1,342.21 | Advertising & marketing |
| Credits | +418,875.71 | customer payments (match to invoices), plus some refunds |

_Exact QuickBooks account names to be checked against the chart of accounts before any rule is made._

## Problems found in the 2026 sheet (2026-10-17)

- **Payroll tab is mostly transfers**: 21 transfers to the payroll share account (-75,380.98). In QuickBooks these are Transfers, not expenses; the expense is the payroll itself from that account.
- **Double counts**: 5/8 cash -500 "Sherwin payment" is in both Draws and Raw Mat; 8/17 ATM -600 "Robs Draw" is in Draws twice; 8/17 PayPal -21.19 in Payroll and Soft; 1/16 cash -700 split $600 draw / $100 truck part but Draws holds the full -700; 2/17 ATM split across Cloth and Draws.
- **Loan repayments**: 2025 loan repayment transfers (5,000 on 4/29, 14,600 on 6/11) were taken out of Draws; they need a loan account in QuickBooks, not an expense or draw. Other debt payments sit in Draws.
- **Personal items in expense tabs** (for SKM to rule on, not deductible as business by default): personal vehicles flagged by Joe's own dashboard ($11,696), some clothing, meals, software and tax-prep rows. Book them as draws unless SKM says otherwise.
- **Merchants that need a human call**: Amazon, Lowe's, Home Depot, Walmart, gas stations, PayPal, cash withdrawals and checks appear in several tabs, so a bank rule can't decide them; they get Joe's note or a receipt.
- Vehicles tab sums to -32,048.14 but the dashboard shows 28,001.60.

## Plan

1. Confirm the tab → account map against QuickBooks' chart of accounts.
2. Bank rules for single-category merchants (Claude in Chrome creates them).
3. Clear the pending bank feed against the sheet; multi-category merchants go to Joe as a short list.
4. Reconcile each account month by month (none was done for about a year).
5. Questions for SKM: personal items, equipment vs expense, the loan account, sales tax on nonprofit customers.

## Rulings from Joe (2026-10-17)

- **One merchant, one category, one payee name, in 2025 and 2026 alike** (Joe: "imperative"). Same merchant must land in the same category both years so the years compare and bank rules work. Merchants that really vary (Amazon, Lowe's, Home Depot, Walmart, gas stations, PayPal, cash, checks) go by receipt or Joe's note and are the only exception.

- **Personal vehicles:** Silverado = Justin's (3102 Partner Distributions – Justin); Lincoln = Joe's (3101). Post as draws, mark SKM review.
- **Partner distribution accounts:** 3101 Joe, 3102 Justin, 3103 Rob. "Withdrawal Transfer J" / "TRANSFER TO J FLETCHER" = Joe's draw unless noted.
- **Chad Henry is paid by paper check** (no direct deposit). His net check is written from checking and the same amount is moved back in from the payroll share account, so the pair is a paycheck plus a transfer, not income.
- **Check 2017, $76 to Chad Henry** = back pay for a $1/hr raise missed for two weeks, paid outside payroll. Book to wages; tell ECAA so it lands on his payroll records and W-2.
- **Customer deposits before 9/30/2026** (no QuickBooks invoices then): income with the customer's name, no invoice.
- Gas-station rows on the Meals tab → Meals; Lowe's on Raw Mat → Cost of goods sold:Material; consumables → Supplies; Clover/FDMS/Bankcd → Merchant account fees.
- **Bank account …0010 "Check Float"** receives "To Share 0010" and "Billscheckssept" transfers from checking.
- **Check Float (…0010)**: a real bank account; QuickBooks account "Check Float (0010)" created for it. "To Share 0010", "Billscheckssept" and "Share Bills Out" are transfers into it.
- **Cell phones** → Utilities:Phone service (Joe's Facilit tab).
- **Floori.io** = the floor visualizer website → Software & apps.
- **Car washes on Joe's personal vehicle** → 3101 draw.
- **Loan from Joe**: Joe has lent the company close to $60,000 over the years. The partners agreed that check 1800 ($2,000, written to Herbe for Joe's personal taxes) is interest on that loan. Booked as Joe's draw with "SKM review" for now: deducting it as interest expense needs a documented loan (balance, rate) and makes it interest income to Joe. **Ask SKM** to set up the loan account and decide.
- **Widget Financial** is the business bank and also Joe's personal bank; only Joe has a personal Widget account. "Fletcherjoseph", "J Fletcher" or "Transfer J" = Joe's draw (3101). **Justin is also a Fletcher**: "Fletcherjustin" = Justin's draw (3102).
- **Card ending 5898 = Justin's** (Widget Financial $500 on 9/26 and $100 on 9/27 → 3102 Justin).
- **West Ridge branch cash withdrawals** are partners' draws: $500 9/26 = Justin (card 5898), $500 10/7 = Rob; $450 10/8 held.
- **Machine/equipment running costs** (propane from Rent-A-Wreck, U-Haul, Tractor Supply; small machine parts) stay in Joe's Mach/Eqip category: use an *expense* account for it (e.g. "Machine & equipment expense"), never the Machinery and Equipment fixed-asset account, which is for buying machines.
- **Country Fair under ~$25–30 = food** (Meals). Rob sometimes buys a $25 gas card there; $25 even = gas.
- **Niagara Machine** can be tools (grinders, tooling) or materials; go by Joe's note. $474.88 on 10/9 = tool (grinder and tooling).
- **Target $146.67 (10/8)** = Keurig coffee maker, creamer and coffee for the shop → Supplies.
- Chick-fil-A and vending (AVI Food) → Meals.
- Chad's paper paychecks pair with a "Share Chads" transfer from the payroll share account (checks 1218, 1221, 222, 229).
- Open with Joe: Check 1785 $1,500; the "Share" transfers (+$3,667.04, +$3,188.98, −$2,000, +$2,000, +$4,367.89); $33.60 extra on the Certified Home Remodelers (Jessup) check; West Ridge $450 (10/8); "Tools" $224.97 (10/15).

## Payroll 2026 (Van Cleve, through 10/9)

- Sheet **"2026 Payroll Register (Van Cleve)"** (Drive, 814 COMMONS / Payroll / Van Cleve), built 10/17 from Liz's emails. Q1 by pay date; Q2 and Q3 quarter totals only; 10/9 run totals. Gross: Q1 20,871.93, Q2 19,228.52, Q3 31,038.79, 10/9 4,942.50. Original PDFs are still only in Outlook.
- Books use the cash method Liz used: Van Cleve net-pay debits → Payroll Expenses:Wages; IRS, PA Revenue, PA UC and Berkheimer payments → Wages Tax Expense; Van Cleve fees → Accounting fees. SKM trues wages up to the W-2s at year end. From 10/23, ECAA's per-run reports allow a proper entry per payroll.
- Joe asked Van Cleve (9/25) to file the **Q3 2026** returns (due 10/31); confirm she did. The 10/9 run is Q4: ECAA needs it for Q4 filings and W-2s.
- **PA UC payment plan** (UC-10A, letter 7/16/2026): 12 monthly installments of $226.05, next due 10/22. PA applied the Q2 2026 UC payment ($249.80) to 1Q 2025, so Q2 2026 shows unpaid. Check that the installments are being paid.
- Aflac: Van Cleve withheld it but did not pay Aflac; 814 pays Aflac's bills directly (Aflac expense in QuickBooks).

## 2025

**Correction (from Joe's email, 2026-09-15):** SKM (David Herbe) filed 2025 "with this information and **will amend once the books are good to go**." So clean 2025 books matter for taxes, not just comparison. Before touching 2025 in QuickBooks, ask SKM how they want it: corrected 2025 in QuickBooks (they asked Liz for the 2025 cash-basis general ledger on 9/18) or a list of adjustments. Do 2026 first either way.
SKM also said (9/17): money a partner puts in for cash flow should be **a loan on the balance sheet**.

- Joe's 2025 sheets (Drive): **"2025 814 EPOXY ExportedTransactions ALL OF"** (sorted into tabs, with a dashboard) and **"2025 ExportedTransactions 2025"** (the raw export, 2,476 rows, one account, full year). Same data; 99.8% sorted (only check #1588, $8,295.78 on 6/2/2025, and three ~$1 charges unsorted).
- 2025 money in +$596,019; out −$610,639.
- 2025 tab → 2026 tab: CreditsPayments→Credits; GasFuel + Fleet Expenses→Vehicles; LiquidsSundries→Shop Supp (check: may be materials); EquipmentToolingMaterials→Raw Mat (split tooling/equipment out); Food→Meals; Employee Checks→Payroll; Owner Checks→Draws; SubscriptionsOffice→Soft; Advertising→Adv; Insurance→Insur; TaxesFees→Taxes/Fees; Utilities→Facilit (its $1,750 checks look like rent → Rent); Rentals→Rent or equipment rental; ATM/Check Withdrawls→by note.
- 2025 propane: Joe decided (10/17) every U-Haul, Rent-A-Wreck and Tractor Supply row in every year goes to Machine & Equipment Expense, 2025 included, so it is one category everywhere. Tell SKM this changes 2025 categories (no change to totals) for the amendment.
- 2025 problems: Fleet rows (−$10,341) also sit in GasFuel, so the dashboard counts fleet spend up to three times (real vehicle spend $36,544); Transfers tab mostly moves to the payroll share; Credits include transfers in, a $15,080 "Paychecks/Salary" item, refunds; Owner Checks include ~$35.8k of transfers to two named people who may be employees, not owners; loan repayment not separated; personal items (groceries in Food; Silverado/Lincoln $3,893); Monthly Summary Rentals and TOTAL rows are wrong.

- 2026-10-17: Checking 1010 down to 8 held rows; savings 1020 to 5 (payroll, waiting on registers). "Machine & Equipment Expense" account created; all propane (Rent-A-Wreck, U-Haul, Tractor Supply), past and future, goes there. Joe: small U-Haul and Tractor Supply charges are propane, not truck rental or materials.
