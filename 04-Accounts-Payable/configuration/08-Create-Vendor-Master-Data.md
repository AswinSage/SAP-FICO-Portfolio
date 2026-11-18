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
| Vendor Account Group | Record from SAP |
| Company Code | Record from SAP |
| Purchasing Organization | Record if applicable |
| Vendor name / number | Use approved or redacted data |
| Reconciliation Account | Record from SAP |
| Payment Terms | Record from SAP |

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