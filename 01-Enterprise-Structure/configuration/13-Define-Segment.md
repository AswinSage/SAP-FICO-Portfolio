# Define Segment

## 1. Objective
Document the Segment definition activity included in the Enterprise Structure phase of the source project.

## 2. Business Purpose
The source describes a Segment as an organizational unit for separate reporting of revenues, expenses, assets, and liabilities across different business activities or areas.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Enterprise Structure → Definition → Financial Accounting → Define Segment`

## 4. Procedure as Written in Source
1. Select New Entries.
2. Enter a four-digit code in the field identified by the source as Functional Area.
3. Enter the Functional Area Name.
4. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Segment identifier | Record from SAP |
| Description / name | Record from SAP |
| Actual fields maintained | Verify in SAP |

## 6. Validation
- [ ] Segment entry is visible in the project system.
- [ ] Identifier and description are confirmed.
- [ ] Actual fields maintained are recorded accurately.
- [ ] Screenshot matches the saved configuration.

## 7. Evidence
Suggested: `13-Define-Segment.png`.

## 8. Source-Document Verification Note
The source labels this activity “Define Segment” but its procedure refers to a code and name in “Functional Area” fields. This is an internal terminology inconsistency in the source document. Do not silently correct it. Confirm the exact configuration object and fields used in the SAP system before publishing this as verified Segment configuration.

## 9. Source Note
Implementation project document, Phase 1, section 1.8.