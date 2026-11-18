# Create Vendor Reconciliation G/L Account

## 1. Objective
Create a G/L account that automatically reflects postings made to vendor sub-ledger accounts.

## 2. Business Purpose
The source explains that reconciliation accounts maintain synchronization between vendor sub-ledger balances and the General Ledger. Direct postings to these accounts are generally restricted.

## 3. Master Data Activity
**SAP navigation:** `SAP Easy Access → Accounting → Financial Accounting → General Ledger → Master Records → G/L Accounts → Individual Processing → Centrally`

## 4. Procedure
1. Enter the Chart of Accounts.
2. Enter the G/L Account Number.
3. Select Create.
4. Enter the Account Group and Description.
5. Select Balance Sheet as the Account Type.
6. Open Control Data.
7. Select Reconciliation Account for Account Type: Vendors.
8. Enter the Company Code.
9. Maintain required company code data.
10. Verify mandatory details and save.

## 5. Project Values
| Field | Project value |
|---|---|
| Chart of Accounts | Record from SAP |
| G/L Account | Record from SAP |
| Account Group | Record from SAP |
| Description | Record from SAP |
| Reconciliation category | Vendors |
| Company Code | Record from SAP |

## 6. Validation
- [ ] Account is created as a Balance Sheet account.
- [ ] Reconciliation category is Vendors.
- [ ] Company code data is maintained.
- [ ] Account is available for vendor master assignment.

## 7. Evidence
Suggested: `06-Create-Vendor-Reconciliation-Account.png`.

## 8. Source Note
Implementation project document, Phase 4, section 4.5.