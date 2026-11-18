# Test Scenario 8.2 – G/L Posting

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.2 G/L Posting |
| Source procedure page | 130 |
| Source screenshot pages | 131–132 |
| Scenario category | Financial transaction validation |
| Execution status | Executed – Completed (project completion confirmed by project owner) |

## Objective

Validate direct and indirect G/L posting, including document header data, debit and credit line items, optional cost object assignments, document balancing, and successful posting.

## Source Procedure

1. Enter the Company Code.
2. Enter Document Date, Posting Date, and Currency.
3. Enter the G/L Account.
4. Select the Debit/Credit Indicator and enter the Amount.
5. Enter Cost Centre and Profit Centre where required.
6. Enter the Document Header Text.
7. Verify the document and post.

## Posting Paths Shown in the Source

| Source screenshot page | Label in source | Reference |
|---:|---|---|
| 131 | Direct Posting | F-02 |
| 132 | Indirect Posting | FB50 |

The companion Business Processes PDF contains a conflicting reference to FS00 for direct G/L posting. In the implementation report, Phase 8 explicitly labels the posting screens F-02 and FB50. FS00 is identified elsewhere as G/L master maintenance, so the discrepancy is not adopted as a Phase 8 posting reference.

## Preconditions

- Required G/L master records exist and are not blocked for the posting activity.
- Posting period is open.
- Document type, number range, posting keys, and tolerance settings are available.
- Relevant cost centre or profit centre exists where account assignment is required.

## Expected Results

- An accounting document is posted in the specified company code and period.
- Debit and credit totals are equal.
- G/L account balances and line items are updated.
- Optional cost centre and profit centre assignments are carried by the relevant line items.
- A document number is generated and the document can be displayed.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Header | Company Code, Document Date, Posting Date, Currency and Header Text are correct |
| Line items | Correct G/L accounts, debit/credit indicators and amounts |
| Balance | Document balance is zero |
| Cost assignment | Required Cost Centre / Profit Centre values are present |
| Posting result | Document posted and document number exists |
| Reporting | Relevant G/L line items are visible in the G/L line-item report |

## Source Screenshot Register

| PDF page | Screenshot subject |
|---:|---|
| 131 | Direct Posting – F-02 |
| 132 | Indirect Posting – FB50 |

## Related Portfolio Scenarios

- [G/L Direct Posting](../../03-General-Ledger/business-processes/02-General-Ledger-Direct-Posting.md)
- [G/L Line-item Report](../../03-General-Ledger/business-processes/08-GL-Line-Item-Report.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.2, pages 130–132.
