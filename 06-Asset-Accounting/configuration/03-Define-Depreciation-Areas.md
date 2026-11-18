# Define Depreciation Areas

## 1. Objective
Document depreciation areas maintained within the Chart of Depreciation.

## 2. Business Purpose
The source describes a Depreciation Area as a valuation view used to calculate and report asset depreciation for different accounting, tax, or reporting requirements.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Asset Accounting → Valuation → Depreciation Areas → Define Depreciation Areas`

## 4. Procedure
1. Select the required Chart of Depreciation.
2. Select the required Depreciation Area.
3. Enter the Description.
4. Define the Depreciation Type.
5. Maintain the Posting Indicator.
6. Maintain the Real Depreciation Area setting, if required.
7. Maintain Currency settings.
8. Verify mandatory details.
9. Save.

## 5. Project Values
| Field | Value visible in SRC-01 |
|---|---|
| Chart of Depreciation | HM11 - Chart of Depreciation - HM11 |
| Depreciation Area | 1 |
| Description | Book depreciation |
| Real Depreciation Area | Selected |
| Posting in G/L | 1 - Area Posts in Realtime |
| Target Ledger Group | Not entered / not visible |
| Alternative Depreciation Area | Not entered / not visible |
| Cross-system depreciation area | Not entered / not visible |

### Value Maintenance Settings Visible in the Screenshot

The screenshot shows **All Values Allowed** for the following entries: Acquisition value, Net book value, Investment grants, Revaluation, Ordinary depreciation, Special depreciation, Unplanned depreciation, Transfer of reserves, Interest, and Revaluation ordinary depreciation.

Source: implementation report, PDF page 87. These are screenshot-visible settings; confirm them in the target system before configuration.

## 6. Validation
- [ ] Correct chart and area are selected.
- [ ] Depreciation type and posting indicator are checked.
- [ ] Currency settings are verified.
- [ ] Saved area can be displayed.

## 7. Evidence
Suggested: `02-Define-Depreciation-Areas.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.2.