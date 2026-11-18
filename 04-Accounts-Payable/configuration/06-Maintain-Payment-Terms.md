# Maintain Payment Terms

## 1. Objective
Define payment conditions used when settling vendor and customer invoices.

## 2. Business Purpose
The source explains that Payment Terms specify due dates, cash discount percentages, and payment periods. They are assigned to customer and vendor master records and support consistent calculation of due dates and discounts.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Business Transactions → Incoming Invoices/Credit Memos → Maintain Terms of Payment`

## 4. Procedure
1. Select New Entries.
2. Enter the four-character payment terms code.
3. Set the discount percentage and number of days.
4. Select the baseline date information.
5. Verify the values.
6. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Payment Terms Key | Record from SAP |
| Description | Record from SAP |
| Discount percentage | Record from SAP |
| Discount days | Record from SAP |
| Baseline date rule | Record from SAP |

## 6. Validation
- [ ] Payment terms key exists.
- [ ] Discount days and percentage are checked.
- [ ] Baseline date information is correct.
- [ ] Terms can be assigned to the relevant vendor master.

## 7. Evidence
Suggested: `05-Maintain-Payment-Terms.png`.

## 8. Source Note
Implementation project document, Phase 4, section 4.4.