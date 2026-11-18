# Create Vendor Master Data

## 1. Objective
Create the vendor master record required for supplier accounting and payment transactions.

## 2. Business Purpose
The source describes vendor master data as containing name, address, communication, company code, accounting/payment, and purchasing information where applicable.

## 3. Master Data Activity
**SAP navigation:** `SAP Easy Access → Accounting → Financial Accounting → Accounts Payable → Master Records → Maintain Centrally → Create`

## 4. Procedure
1. Enter the Vendor Account Group.
2. Enter the Company Code.
3. Enter the Purchasing Organization, if required.
4. Press Enter.
5. Maintain Address and Communication details.
6. Enter the Reconciliation Account and Payment Terms in Company Code Data.
7. Maintain Purchasing Data, if applicable.
8. Verify mandatory details.
9. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Field | Value visible in SRC-01, PDF page 60 |
|---|---|
| Vendor name | Infineon Technologies |
| Vendor number | 2026202601 |
| Company Code | HM11 - Hindustan Motors Ltd |
| Reconciliation Account | 1002 |
| Sort Key | 001 |
| Street / House number | Harpy Street / 512 |
| City / Country | Chennai / IN |
| Postal Code / PO Box | 600018 / 600018 |
| Region | 22 |
| Language | EN - English |
| Vendor Account Group | Not visible in the screenshot |
| Purchasing Organization | Not visible in the screenshot |
| Payment Terms | Not visible in the screenshot |

The implementation report also names Analog Devices Ltd as a foreign vendor example for HM12 (SRC-01, PDF page 61). The separate business-process PDF uses BE Solution Pvt Ltd and Sun IT Solutions in its vendor examples; do not merge these sample records. Use vendor details in public only when permitted.

## 6. Validation
- [ ] Vendor master is created.
- [ ] General data is complete.
- [ ] Company code data is complete.
- [ ] Reconciliation account and payment terms are correct.
- [ ] Purchasing data is maintained only if applicable.
- [ ] Vendor can be selected for invoice posting.

## 7. Evidence
Suggested: `07-Create-Vendor-Master-Data.png`.

## 8. Source Note
Implementation project document, Phase 4, section 4.6.