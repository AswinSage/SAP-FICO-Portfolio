# Test Scenario 8.6 – Customer Invoice

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.6 Customer Invoice |
| Source procedure page | 142 |
| Source screenshot page | 143 |
| Scenario category | Accounts Receivable transaction validation |
| Execution in current target environment | Not independently verified |

## Objective

Validate customer invoice posting for goods or services, including customer receivable recognition, revenue posting, optional tax, and the customer / General Ledger integration.

## Source Procedure

1. Enter the Company Code and Customer Account.
2. Enter Invoice Date, Posting Date, Invoice Amount, and Currency.
3. Enter the Revenue G/L Account and the G/L line-item amount.
4. Enter Tax Code where applicable.
5. Enter Cost Centre or Profit Centre where required.
6. Confirm that the document Balance is Zero.
7. Post the invoice.

## Preconditions

- Customer master exists with company-code data and customer reconciliation account.
- Revenue G/L account exists.
- Posting period and document controls are active.
- Tax code and cost object assignments are available where applicable.

## Expected Results

- Customer receivable is recognised in the customer sub-ledger.
- Revenue is recorded in the relevant G/L account.
- Output tax is recorded where applicable and configured.
- Document debits and credits balance to zero.
- Customer open item is available for subsequent receipt and clearing.
- Customer and G/L line-item reports reflect the invoice.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Customer | Correct customer and company code |
| Invoice header | Invoice date, posting date, amount and currency are correct |
| Revenue | Correct revenue G/L account and amount |
| Tax | Tax entry is present only where applicable |
| Cost assignment | Required Cost Centre / Profit Centre is present |
| Balance | Zero document balance |
| Sub-ledger | Customer open item is created |
| G/L integration | Customer reconciliation and revenue entries reflect the invoice |

## Source Screenshot Register

Page 143 contains the customer invoice posting screens.

## Related Portfolio Scenarios

- [Create Customer Master Data](../../05-Accounts-Receivable/business-processes/14-Create-Customer-Master-Data.md)
- [Customer Invoice](../../05-Accounts-Receivable/business-processes/17-Customer-Invoice.md)
- [Customer Line-item Report](../../05-Accounts-Receivable/business-processes/19-Customer-Line-Item-Report.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.6, pages 142–143.
