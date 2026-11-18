# Define Account Determination Key

## 1. Objective
Define the Account Determination Key used to link asset classes with relevant G/L accounts.

## 2. Business Purpose
The source explains that the key determines the G/L accounts used for asset acquisition, depreciation, retirement, and other asset-related transactions. It is assigned to the relevant asset class.

## 3. Configuration Activity
**SAP navigation:** `SPRO → IMG → Financial Accounting → Asset Accounting → Organizational Structure → Asset Class → Specify Account Determination`

## 4. Procedure
1. Open the Account Determination activity.
2. Select New Entries.
3. Enter the Account Determination Key.
4. Enter the name of the account determination.
5. Save.

## 5. Project Values
| Account Determination Key | Description visible in SRC-01, PDF page 99 |
|---|---|
| HM11 | Machine |
| HM12 | Building |
| HM13 | Vehicle |

The same screenshot shows Chart of Depreciation HM11 and Chart of Accounts HM11. Additional keys are visible lower in the on-screen list; this table records only the first three clearly legible entries. Confirm the full list and asset-class assignments in the target system.

## 6. Validation
- [ ] Key is created.
- [ ] Description is correct.
- [ ] Key is available for assignment to the relevant asset class.

## 7. Evidence
Suggested: `03-Define-Account-Determination-Key.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.3.