# Create Vendor Number Range

## 1. Objective
Define the number interval used for vendor master account numbers.

## 2. Business Purpose
The source explains that vendor number ranges support internal assignment by the system or external assignment entered by the user. They provide systematic and unique vendor identification.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Vendor Accounts → Master Data → Preparations for Creating Vendor Master Data → Create Number Ranges for Vendor Accounts`

## 4. Procedure
1. Select Change Intervals.
2. Select Insert Interval.
3. Enter the Number Range identifier.
4. Enter the From Number.
5. Enter the To Number.
6. Select External if external number assignment is required.
7. Verify the interval.
8. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Number Range | Record from SAP |
| From Number | Record from SAP |
| To Number | Record from SAP |
| Internal / External | Record actual selection |

## 6. Validation
- [ ] Interval is defined.
- [ ] From and To values are valid.
- [ ] Internal/external assignment matches the project design.
- [ ] Interval can be displayed after saving.

## 7. Evidence
Suggested: `02-Create-Vendor-Number-Range.png`.

## 8. Source Note
Implementation project document, Phase 4, section 4.2.