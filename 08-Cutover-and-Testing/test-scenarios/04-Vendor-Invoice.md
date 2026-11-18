# Test Scenario 8.4 – Vendor Invoice

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.4 Vendor Invoice |
| Source procedure page | 135 |
| Source screenshot pages | 136–138 |
| Scenario category | Accounts Payable transaction validation |
| Execution status | Executed – Completed |

## Objective

Validate vendor invoice posting, including liability recognition, corresponding expense or asset entry, tax where applicable, and the resulting vendor and General Ledger line items.

## Direct PDF Page Links

- **Procedure:** [PDF p.135](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=135)
- **Screenshots:** [PDF p.136](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=136) · [PDF p.137](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=137) · [PDF p.138](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=138)

## Source Procedure

1. Enter the Company Code and Vendor Account.
2. Enter Invoice Date, Posting Date, and Invoice Amount.
3. Enter the Tax Code where applicable.
4. Enter the Expense or G/L Account.
5. Enter the amount for the G/L line item.
6. Enter Cost Centre where required.
7. Confirm that the document Balance is Zero.
8. Post the invoice.

## Posting Reference Shown in the Source

| PDF page | Screenshot caption |
|---:|---|
| 136 | Direct Posting – F-02 |
| 137 | Indirect Posting – FB60 |
| 138 | Additional document / posting display |


## Preconditions

- Vendor master exists with company-code accounting data and a vendor reconciliation account.
- Expense or asset G/L account exists.
- Posting period and required document controls are active.
- Tax code is available where tax is part of the transaction.
- Required cost centre exists where account assignment is necessary.

## Expected Results

- Vendor liability is recorded in the vendor sub-ledger.
- Corresponding expense or asset value is recorded in the G/L.
- Input tax is recorded where applicable and configured.
- Document debits and credits balance to zero.
- Vendor open item is available for payment and clearing.
- Vendor and G/L line-item reports reflect the invoice.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Vendor | Correct vendor and company code |
| Invoice header | Invoice date, posting date, reference and amount are correct |
| Expense / asset | Correct G/L account and amount |
| Tax | Tax entry is present only where applicable |
| Balance | Zero document balance |
| Sub-ledger | Vendor open item is created |
| G/L integration | Reconciliation account and expense / asset entries reflect the invoice |

## Source Screenshot Register

Pages 136–138 contain the invoice-related SAP screen states and posting display.

## Related Portfolio Scenarios

- [Create Vendor Master Data](../../04-Accounts-Payable/business-processes/09-Create-Vendor-Master-Data.md)
- [Vendor Rent Invoice](../../04-Accounts-Payable/business-processes/11-Vendor-Invoice-Rent.md)
- [Vendor Line-item Report](../../04-Accounts-Payable/business-processes/13-Vendor-Line-Item-Report.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.4, pages 135–138.
