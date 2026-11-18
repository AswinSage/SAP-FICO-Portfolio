# Assign Customer Account Group to Number Range

## 1. Objective
Document the assignment of a customer account group to its number range.

## 2. Business Purpose
The source describes this assignment as determining the number interval used when creating customer master records and controlling internal or external number assignment.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Customer Accounts → Master Data → Preparations for Creating Customer Master Data → Define Account Groups with Screen Layout (Customers)`

## 4. Procedure
1. Open the customer account group assignment activity.
2. Select the required Customer Account Group.
3. Enter the corresponding Number Range.
4. Verify the number range assignment.
5. Ensure the interval is valid for the account group.
6. Save.

## 5. Project Values
| Field | Project value |
|---|---|
| Customer Account Group | Record from SAP |
| Number Range | Record from SAP |
| Assignment result | Pending verification |

## 6. Validation
- [ ] Correct customer account group is selected.
- [ ] Intended number range is assigned.
- [ ] Assignment is saved and can be displayed.
- [ ] Customer master creation follows the expected numbering behavior, if tested.

## 7. Evidence
Suggested: `04-Assign-Customer-Account-Group-Number-Range.png`.

## 8. Source Note
Implementation project document, Phase 5, section 5.3.1.