# Create Customer Reconciliation G/L Account

## 1. Objective
Create a G/L account linked to the customer sub-ledger for customer receivable postings.

## 2. Business Purpose
The source explains that customer postings automatically update the reconciliation account in the General Ledger. Direct postings are generally restricted to maintain sub-ledger integrity.

## 3. Master Data Activity
**SAP navigation:** `SAP Easy Access → Accounting → Financial Accounting → General Ledger → Master Records → G/L Accounts → Individual Processing → Centrally`

## 4. Procedure
1. Enter the Chart of Accounts.
2. Enter the G/L Account Number.
3. Select Create.
4. Enter the Account Group.
5. Enter the G/L Account Description.
6. Select Balance Sheet Account as the Account Type.
7. Open Control Data.
8. Select Reconciliation Account for Account Type – Customers.
9. Enter the Company Code.
10. Maintain the required Field Status Group.
11. Verify and save.

## 5. Project Values
| Field | Project value |
|---|---|
| Chart of Accounts | Record from SAP |
| G/L Account | Record from SAP |
| Account Group | Record from SAP |
| Description | Record from SAP |
| Reconciliation category | Customers |
| Company Code | Record from SAP |
| Field Status Group | Record from SAP |

## 6. Validation
- [ ] Account type is Balance Sheet.
- [ ] Reconciliation category is Customers.
- [ ] Company code data is maintained.
- [ ] Account is available for customer master assignment.

## 7. Evidence
Suggested: `06-Create-Customer-Reconciliation-Account.png`.

## 8. Source Note
Implementation project document, Phase 5, section 5.5.