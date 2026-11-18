# Create Customer Number Range

## 1. Objective
Define the interval used to assign customer account numbers.

## 2. Business Purpose
The source explains that customer number ranges support internal or external number assignment and systematic identification of customer master records.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Customer Accounts → Master Data → Preparations for Creating Customer Master Data → Create Number Ranges for Customer Accounts`

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
- [ ] Number assignment type matches the project design.
- [ ] Interval can be displayed after saving.

## 7. Evidence
Suggested: `02-Create-Customer-Number-Range.png`.

## 8. Source Note
Implementation project document, Phase 5, section 5.2.