# Maintain Cost Element

## 1. Objective
Document cost element maintenance for classifying costs and revenues in management accounting.

## 2. Business Purpose
The source describes Cost Element Accounting as connecting financial accounting postings with Controlling objects such as Cost Centres and Internal Orders, supporting allocation, planning, analysis, and internal reporting.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Controlling → Cost Element Accounting → Master Data → Cost Elements → Automatic Creation of Cost Elements`

## 4. Procedure
1. Enter the Controlling Area.
2. Enter the Cost Element.
3. Enter the Valid From date.
4. Enter the Valid To date.
5. Select the Cost Element Category.
6. Enter the Description.
7. Maintain the Default Account Assignment, if applicable.
8. Verify mandatory details.
9. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Controlling Area | Record from SAP |
| Cost Element | Record from SAP |
| Valid From / To | Record from SAP |
| Cost Element Category | Record from SAP |
| Description | Record from SAP |
| Default Account Assignment | Record if applicable |

## 6. Validation
- [ ] Cost Element exists.
- [ ] Validity dates are correct.
- [ ] Category and description are checked.
- [ ] Default account assignment is verified where used.
- [ ] Cost element is available for relevant CO postings.

## 7. Evidence
Suggested: `07-Maintain-Cost-Element-Repair-Charge.png`, `07-Maintain-Cost-Element-Maintenance-Charge.png`, `07-Maintain-Cost-Element-Internal-Settlement.png`.

## 8. Source Note
Implementation project document, Phase 7, section 7.4.