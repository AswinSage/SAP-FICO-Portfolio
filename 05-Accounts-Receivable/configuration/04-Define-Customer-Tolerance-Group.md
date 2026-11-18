# Define Customer Tolerance Group

## 1. Objective
Define limits for payment differences and cash discount adjustments during customer clearing.

## 2. Business Purpose
The source describes Customer Tolerance Groups as controlling permitted differences in amounts and percentages for transactions and open items, together with cash discount adjustments.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Customer Accounts → Business Transactions → Incoming Payments → Incoming Payments Global Settings → Define Tolerance Groups for Customers`

## 4. Procedure
1. Select New Entries.
2. Enter the Tolerance Group.
3. Enter the Description, if required.
4. Enter the Amount per Document.
5. Enter the Amount per Open Item.
6. Maintain the Permitted Payment Difference.
7. Maintain Cash Discount Adjustment, if required.
8. Verify mandatory details.
9. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Tolerance Group | Record from SAP |
| Description | Record from SAP |
| Amount per Document | Record from SAP |
| Amount per Open Item | Record from SAP |
| Permitted Payment Difference | Record from SAP |
| Cash Discount Adjustment | Record if used |

## 6. Validation
- [ ] Tolerance group exists.
- [ ] Amount limits are correct.
- [ ] Payment difference settings are checked.
- [ ] Cash discount adjustment is checked where used.
- [ ] Saved settings can be displayed.

## 7. Evidence
Suggested: `03-Define-Customer-Tolerance-Group.png`.

## 8. Source Note
Implementation project document, Phase 5, section 5.3.