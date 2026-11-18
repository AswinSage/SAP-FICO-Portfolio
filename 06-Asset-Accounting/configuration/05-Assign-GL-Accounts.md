# Assign G/L Accounts for Asset Accounting

## 1. Objective
Document assignment of G/L accounts to asset accounting transaction keys using the Account Determination Key.

## 2. Business Purpose
The source describes this assignment as connecting asset accounting transactions with the appropriate General Ledger accounts for acquisition, accumulated depreciation, depreciation expense, and retirement where required.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Asset Accounting → Integration with General Ledger Accounting → Assign G/L Accounts`

## 4. Procedure
1. Enter the Chart of Accounts.
2. Select the Account Determination Key.
3. Select the required Transaction Key.
4. Enter the relevant G/L Account.
5. Maintain accounts for Asset Acquisition.
6. Maintain accounts for Accumulated Depreciation.
7. Maintain accounts for Depreciation Expense.
8. Maintain accounts for Asset Retirement, if required.
9. Verify all account assignments.
10. Save.

## 5. Project Values
| Assignment | Project G/L account |
|---|---|
| Asset Acquisition | Record from SAP |
| Accumulated Depreciation | Record from SAP |
| Depreciation Expense | Record from SAP |
| Asset Retirement | Record if applicable |

Also record the Chart of Accounts, Account Determination Key, and Transaction Keys actually used.

## 6. Validation
- [ ] Correct Chart of Accounts is selected.
- [ ] Account Determination Key is correct.
- [ ] Required transaction keys are maintained.
- [ ] G/L account assignments are valid.
- [ ] Asset posting test confirms expected account determination, if performed.

## 7. Evidence
Suggested: `04-Assign-Asset-Accounting-GL-Accounts.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.7.3.