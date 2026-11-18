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
| Field | Value visible in SRC-01, PDF page 94 |
|---|---|
| Chart of Depreciation | HM11 |
| Depreciation Key | HM11 |
| Description | The screenshot header shows Chart of Depreciation - HM11; no separate key description is clearly visible |
| Status | Inactive |
| Depreciation Type | N - Ordinary depreciation |
| Phase | 1 - From the start of depreciation |
| Base Method | 001 |
| Declining-Balance Method | 001 |
| Period Control Method | 001 |
| Multilevel Method | 001 |
| Class | 0 - No assignment |
| Multiple Shift | Increase in depreciation and expired useful life |
| Scrap Value | 0 - Consideration is controlled by custom value key |
| Acquisition allowed in capitalization year | No |
| Shutdown | No |

The screenshot also shows other control checkboxes (including special depreciation and period-control options) not selected. The status is visibly **Inactive**; do not treat this key as ready for asset postings until its intended status and configuration are confirmed in the target system.

## 6. Validation
- [ ] Depreciation Key exists.
- [ ] Base and period control methods are checked.
- [ ] Optional methods are documented if used.
- [ ] Depreciation Key is available in the relevant depreciation area.

## 7. Evidence
Suggested: `08-Maintain-Depreciation-Key.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.7.