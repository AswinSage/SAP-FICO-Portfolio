# Test Scenario 8.7 – Customer Payment

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.7 Customer Payment |
| Source procedure page | 144 |
| Source screenshot page | 145 |
| Scenario category | Accounts Receivable receipt and clearing |
| Execution status | Executed – Completed (project completion confirmed by project owner) |

## Objective

Validate receipt of a customer payment against an outstanding customer invoice, including bank/cash posting, open-item assignment, and clearing.

## Source Procedure

1. Enter the Company Code, Document Date, Posting Date, and Currency.
2. Enter the Bank/Cash G/L Account and Amount Received.
3. Enter the Customer Account.
4. Select Process Open Items.
5. Select the relevant Customer Invoice.
6. Verify that Assigned Amount and Amount Entered are balanced.
7. Post the receipt.

## Preconditions

- Customer account exists.
- Customer invoice is posted and available as an open item.
- Bank/Cash G/L account is available.
- Incoming-payment and clearing configuration is active.
- Relevant posting period is open.

## Expected Results

- Bank/cash balance increases by the amount received.
- Customer receivable decreases by the receipt amount.
- Selected customer invoice is cleared when fully settled.
- Any residual open balance follows the selected clearing method.
- Payment document and customer clearing status are available for review.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Payment header | Company Code, dates and Currency are correct |
| Bank/cash account | Correct G/L account is selected |
| Customer | Correct customer account is selected |
| Open item | Intended customer invoice is selected |
| Assignment | Assigned Amount equals Amount Received |
| Posting result | Incoming payment document is generated |
| Clearing | Invoice clearing status and remaining balance are correct |

## Source Screenshot Register

Page 145 contains the incoming payment and resulting posting screens.

## Related Portfolio Scenarios

- [Customer Invoice](../../05-Accounts-Receivable/business-processes/17-Customer-Invoice.md)
- [Customer Payment](../../05-Accounts-Receivable/business-processes/18-Customer-Payment.md)
- [Customer Line-item Report](../../05-Accounts-Receivable/business-processes/19-Customer-Line-Item-Report.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.7, pages 144–145.
