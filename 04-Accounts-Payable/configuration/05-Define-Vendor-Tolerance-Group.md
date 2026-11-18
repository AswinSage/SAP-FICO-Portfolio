# Define Vendor Tolerance Group

## 1. Objective
Define permitted payment differences and cash discount adjustments for vendor processing.

## 2. Business Purpose
The source describes Vendor Tolerance Groups as setting acceptable payment differences and cash discount adjustments during vendor invoice processing and clearing.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Business Transactions → Outgoing Payments → Automatic Outgoing Payments → Define Tolerance Groups for Vendors`

## 4. Procedure
1. Select New Entries.
2. Enter the Tolerance Group.
3. Enter the Description, if available.
4. Maintain the Permitted Payment Difference.
5. Maintain the Permitted Payment Difference percentage, if required.
6. Maintain Cash Discount Adjustment, if required.
7. Verify mandatory details.
8. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Tolerance Group | Record from SAP |
| Description | Record from SAP |
| Permitted payment difference | Record from SAP |
| Permitted difference (%) | Record from SAP, if used |
| Cash discount adjustment | Record from SAP, if used |

## 6. Validation
- [ ] Tolerance group exists.
- [ ] Limits match the approved project design.
- [ ] Optional percentage and cash discount settings are checked.
- [ ] Saved settings can be displayed.

## 7. Evidence
Suggested: `04-Define-Vendor-Tolerance-Group.png`.

## 8. Source Note
Implementation project document, Phase 4, section 4.3.