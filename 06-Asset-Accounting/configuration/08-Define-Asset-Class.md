# Define Asset Class

## 1. Objective
Document the Asset Class used to group assets with similar characteristics and accounting requirements.

## 2. Business Purpose
The source describes an Asset Class as controlling important master-data settings such as number ranges, screen layouts, and account determination. It supports consistent depreciation and accounting treatment for similar assets.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Asset Accounting → Master Data → Asset Classes → Define Asset Classes`

## 4. Procedure as Listed in Source
1. Enter the Company Code.
2. Enter the Number Range.
3. Enter the From and To number.
4. Save.

The source procedure is brief. Capture any additional fields and assignments actually maintained in the project system rather than assuming they were configured.

## 5. Project Values
| Field | Project value |
|---|---|
| Asset Class | Record from SAP |
| Description | Record from SAP |
| Company Code context | Record from SAP |
| Number Range | Record from SAP |
| Screen Layout | Record from SAP |
| Account Determination Key | Record from SAP |

## 6. Validation
- [ ] Asset Class exists.
- [ ] Description is correct.
- [ ] Number range assignment is checked.
- [ ] Screen layout and account determination assignments are checked.
- [ ] Asset master can be created using the class, if tested.

## 7. Evidence
Suggested: `07-Define-Asset-Class.png`.

## 8. Source Note
Implementation project document, Phase 6, section 6.6.