# Maintain Cost Centre

## 1. Objective
Document Cost Centre master maintenance for organizational cost collection and reporting.

## 2. Business Purpose
The source describes Cost Centre Accounting as supporting identification, collection, planning, monitoring, allocation, and reporting of costs by department or responsibility area.

## 3. Configuration / Master Data Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Controlling → Cost Center Accounting → Master Data → Cost Centers → Basic Data → Maintain Cost Center`

## 4. Procedure
1. Enter the Controlling Area.
2. Enter the Cost Center.
3. Enter the Validity Date.
4. Open Master Data.
5. Enter the Cost Center Name.
6. Enter the Description.
7. Enter the Person Responsible.
8. Select the Cost Center Category.
9. Enter the Profit Center, if required.
10. Maintain the Functional Area, if required.
11. Verify mandatory details.
12. Save.

## 5. Project Values
| Cost Centre | HM11-1 | HM11-2 |
|---|---|---|
| Description | Production | Marketing |
| Controlling Area | HM11 | HM11 |
| Valid From | 01.04.2026 | 01.04.2026 |
| Valid To | 31.12.9999 | 31.12.9999 |
| Person Responsible label | Production Manager | Marketing Manager |
| Cost Centre Category | 1 - Production | P - Marketing |
| Hierarchy Area | HM11-1 | HM11-1 |
| Business Area | HM21 | HM21 |
| Functional Area | HM11 - Manufacturing | HM11 - Manufacturing |
| Currency | INR | INR |
| Profit Centre | HM11 | HM12 |

Source: implementation report, PDF pages 117-118. The responsible-person fields are role labels shown in the screenshots, not verified employee identities. Validate the Functional Area assignment because both examples display the same Manufacturing functional area.

## 6. Validation
- [ ] Cost Centre exists for the intended validity period.
- [ ] Responsible person and category are checked.
- [ ] Profit Centre and Functional Area assignments are checked where applicable.
- [ ] Cost Centre can be used in relevant postings.

## 7. Evidence
Suggested: `06-Maintain-Cost-Centre-Production.png` and corresponding department records.

## 8. Source Note
Implementation project document, Phase 7, section 7.3.