# Test Scenario 8.5 – Vendor Payment

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.5 Vendor Payment |
| Source procedure page | 139 |
| Source screenshot pages | 140–141 |
| Scenario category | Accounts Payable payment and clearing |
| Execution status | Executed – Completed |

## Objective

Validate outgoing vendor payment against an outstanding vendor invoice, including bank/cash posting, open-item selection, payment assignment, and clearing.

## Source Procedure

1. Enter the Company Code, Document Date, Posting Date, and Currency.
2. Enter the Bank/Cash G/L Account and Payment Amount.
3. Enter the Vendor Account.
4. Select Process Open Items.
5. Select the relevant Vendor Invoice.
6. Verify that Assigned Amount and Amount Entered are balanced.
7. Post the payment.

## Preconditions

- Vendor account exists.
- Vendor invoice is posted and appears as an open item.
- Bank/Cash G/L account is available.
- Payment and clearing configuration is active.
- Relevant posting period is open.

## Expected Results

- Vendor liability is reduced by the payment amount.
- Bank/cash account is credited by the payment amount.
- Selected vendor open item is cleared when fully settled.
- Any remaining balance is represented according to the payment scenario and clearing method.
- Payment document and vendor clearing status are available for review.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Payment header | Company Code, dates and Currency are correct |
| Bank/cash account | Correct G/L account is selected |
| Vendor | Correct vendor account is selected |
| Open item | Intended vendor invoice is selected |
| Assignment | Assigned Amount equals Amount Entered |
| Posting result | Payment document is generated |
| Clearing | Invoice clearing status and remaining balance are correct |

## Source Screenshot Register

Pages 140–141 contain the outgoing payment and resulting posting screens.

## Related Portfolio Scenarios

- [Vendor Rent Invoice](../../04-Accounts-Payable/business-processes/11-Vendor-Invoice-Rent.md)
- [Vendor Payment](../../04-Accounts-Payable/business-processes/12-Vendor-Payment.md)
- [Vendor Line-item Report](../../04-Accounts-Payable/business-processes/13-Vendor-Line-Item-Report.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.5, pages 139–141.
