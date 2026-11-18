# Assign Vendor Account Group to Number Range

## 1. Objective
Document the assignment linking a Vendor Account Group to its number range.

## 2. Business Purpose
The assignment determines which vendor number interval is available when vendor master records are created for the selected account group. The source notes that internal and external assignment may be supported.

## 3. Configuration Activity
**Source navigation note:** The implementation document's navigation text points to Customer Accounts / Customer Master Data even though the section is Vendor Account Group assignment. Treat that path as an inconsistency requiring verification.

## 4. Procedure
1. Open the vendor account group-to-number-range assignment activity confirmed in the project system.
2. Select the required Vendor Account Group.
3. Enter the corresponding Number Range.
4. Verify that the interval is valid for the account group.
5. Save the assignment.

## 5. Project Values
| Field | Project value |
|---|---|
| Vendor Account Group | Record from SAP |
| Number Range | Record from SAP |
| Assignment result | Pending verification |

## 6. Validation
- [ ] Correct vendor account group is selected.
- [ ] Intended number range is assigned.
- [ ] Assignment is saved and can be displayed.
- [ ] Vendor master creation uses the expected numbering behavior, if tested.

## 7. Evidence
Suggested: `03-Assign-Vendor-Account-Group-Number-Range.png`.

## 8. Implementation Notes
Do not silently substitute a generic navigation path. Record the exact path used in the project system.

## 9. Source Note
Implementation project document, Phase 4, section 4.3.1.