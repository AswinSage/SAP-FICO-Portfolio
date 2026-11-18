# Maintain Controlling Area

## 1. Objective
Maintain the Controlling Area used for management accounting and cost control.

## 2. Business Purpose
The source describes the Controlling Area as an organizational unit grouping one or more company codes under a common structure for internal cost accounting, planning, and reporting. It provides the framework for cost centers, internal orders, and profit centers.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Controlling → General Controlling → Organization → Maintain Controlling Area`

## 4. Procedure
1. Select New Entries.
2. Enter the four-character Controlling Area.
3. Enter the Name.
4. Enter the Currency Type.
5. Enter the Currency.
6. Enter the Fiscal Year Variant.
7. Select the Chart of Accounts.
8. Select the Assignment of Company Codes option.
9. Assign the required Company Codes.
10. Verify mandatory details.
11. Save.

## 5. Project Values
| Field | Value visible in SRC-01 |
|---|---|
| Controlling Area | HM11 |
| Name | Controlling Area for HM11 |
| Validity shown | 2026 to 9999 |
| Company Code assignment | 1 - Controlling area same as company code |
| Currency Type | 10 - Company Code Currency |
| Currency | INR |
| Fiscal Year Variant | HM (Jan-Dec) |
| Chart of Accounts | HM11 |
| Standard Hierarchy field | HM11-1 (as legible in the screenshot) |
| Active components | Cost Centers; Profit Center Accounting selected |
| Other indicator | All Currencies selected |

Source: implementation report, PDF page 112. Revalidate the fiscal-year and standard-hierarchy assignments in the target system.

## 6. Validation
- [ ] Controlling Area exists.
- [ ] Currency type and currency are correct.
- [ ] Fiscal Year Variant and Chart of Accounts are checked.
- [ ] Required company codes are assigned.
- [ ] Saved configuration can be displayed.

## 7. Evidence
Suggested: `01-Maintain-Controlling-Area.png`.

## 8. Source Note
Implementation project document, Phase 7, section 7.1.