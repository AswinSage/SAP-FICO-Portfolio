# Maintain Depreciation Key

## 1. Objective
Document the Depreciation Key used to determine asset depreciation calculation rules.

## 2. Business Purpose
The source explains that a Depreciation Key defines the depreciation method, calculation method, and rules used to determine depreciation values, including the depreciation start period based on period control.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Asset Accounting → Depreciation → Valuation Methods → Depreciation Keys → Maintain Depreciation Keys`

## 4. Procedure
1. Enter the Depreciation Key.
2. Enter the Description.
3. Select the Base Method.
4. Select the Declining-Balance Method, if required.
5. Maintain the Period Control Method.
6. Maintain the Multilevel Method, if required.
7. Maintain Depreciation Start Date settings.
8. Verify all depreciation calculation rules.
9. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Depreciation Key | Record from SAP |
| Description | Record from SAP |
| Base Method | Record from SAP |
| Declining-Balance Method | Record if used |
| Period Control Method | Record from SAP |
| Multilevel Method | Record if used |
| Depreciation Start Date settings | Record from SAP |

## 6. Validation
- [ ] Depreciation Key exists.
- [ ] Base and period control methods are checked.
- [ ] Optional methods are documented if used.
- [ ] Depreciation Key is available in the relevant depreciation area.

## 7. Evidence
Suggested: `08-Maintain-Depreciation-Key.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.7.