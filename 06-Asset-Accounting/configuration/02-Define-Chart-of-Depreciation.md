# Define Chart of Depreciation

## 1. Objective
Document the Chart of Depreciation used as the framework for asset valuation and depreciation.

## 2. Business Purpose
The source describes the Chart of Depreciation as containing depreciation areas and valuation rules. It states that each company code is assigned to one Chart of Depreciation, which may contain multiple depreciation areas.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Asset Accounting → Organizational Structures → Copy Reference Chart of Depreciation/Depreciation Areas`

## 4. Procedure
1. Select the Reference Chart of Depreciation.
2. Select Copy.
3. Enter the Target Chart of Depreciation.
4. Enter the Description.
5. Enter the Country.
6. Maintain the required Depreciation Areas.
7. Delete depreciation areas that are not required.
8. Verify the copied settings.
9. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Reference Chart of Depreciation | Record from SAP |
| Target Chart of Depreciation | Record from SAP |
| Description | Record from SAP |
| Country | Record from SAP |
| Depreciation Areas retained | Record from SAP |

## 6. Validation
- [ ] Target chart exists.
- [ ] Description and country are correct.
- [ ] Required depreciation areas are present.
- [ ] Unneeded areas are removed as per design.
- [ ] Copied settings are reviewed.

## 7. Evidence
Suggested: `01-Define-Chart-of-Depreciation.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.1.