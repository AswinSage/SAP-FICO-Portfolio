# Assign Company Code Tax Codes

## 1. Objective
Document tax code settings referenced in the Asset Accounting phase of the implementation report.

## 2. Business Purpose
The source describes tax code configuration as enabling tax calculation during financial transactions and supporting input and output tax recording.

## 3. Configuration Activity
**SAP navigation as listed in source:** `SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Tax on Sales/Purchases → Basic Settings → Check Calculation Procedure`

## 4. Procedure as Listed in Source
1. Enter the Country.
2. Enter the Tax Code.
3. Enter the Tax Code Description.
4. Select the appropriate Tax Type.
5. Maintain the required Tax Rates.
6. Verify the tax code settings.
7. Assign the tax code to the relevant Company Code, as required.
8. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Country | Record from SAP |
| Tax Code | Record from SAP |
| Description | Record from SAP |
| Tax Type | Record from SAP |
| Tax Rate | Record from SAP |
| Company Code | Record from SAP |

## 6. Validation
- [ ] Country and tax code are correct.
- [ ] Tax type and rate are checked.
- [ ] Company code relevance is verified.
- [ ] Tax calculation is tested only if evidence exists.

## 7. Evidence
Suggested: `10-Company-Code-Tax-Code-Settings.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.7.1. The source section title and navigation describe tax code setup; verify the exact assignment activity used in the system.