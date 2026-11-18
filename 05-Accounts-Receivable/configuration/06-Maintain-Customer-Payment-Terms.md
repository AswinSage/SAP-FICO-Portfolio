# Maintain Customer Payment Terms

## 1. Objective
Define payment conditions used to calculate customer invoice due dates and cash discounts.

## 2. Business Purpose
The source explains that payment terms determine payment due dates based on the baseline date and may include cash discount periods and percentages. They are assigned to master records and used during invoice processing.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Business Transactions → Incoming Invoices/Credit Memos → Maintain Terms of Payment`

## 4. Procedure
1. Select New Entries.
2. Enter the Payment Terms Key.
3. Enter the Description.
4. Select the Account Type, if required.
5. Select the Baseline Date for payment calculation.
6. Enter the Cash Discount Days.
7. Enter the Cash Discount Percentage.
8. Enter the Net Due Days.
9. Maintain additional payment conditions, if required.
10. Verify mandatory details and save.

## 5. Project Values
| Field | Project value |
|---|---|
| Payment Terms Key | Record from SAP |
| Description | Record from SAP |
| Account Type | Record if applicable |
| Baseline Date | Record from SAP |
| Cash Discount Days | Record from SAP |
| Cash Discount Percentage | Record from SAP |
| Net Due Days | Record from SAP |

## 6. Validation
- [ ] Payment terms key exists.
- [ ] Baseline date rule is correct.
- [ ] Discount days and percentage are checked.
- [ ] Net due days are checked.
- [ ] Terms can be assigned to customer master data.

## 7. Evidence
Suggested: `05-Maintain-Customer-Payment-Terms.png`.

## 8. Source Note
Implementation project document, Phase 5, section 5.4.