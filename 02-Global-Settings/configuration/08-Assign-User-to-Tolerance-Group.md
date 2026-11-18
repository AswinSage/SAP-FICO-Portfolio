# Assign User Name to Tolerance Group

## 1. Objective

Document the assignment of a user name to an employee Tolerance Group.

## 2. Business Purpose

The source project describes this assignment as the step that applies the posting limits of a tolerance group to a specific accounting user. It supports the allocation of financial processing limits according to user responsibilities.

## 3. Configuration Activity

**Configuration item:** Assign User Name to Tolerance Group for Employees

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Documents → Tolerance Groups → Define Tolerance Groups for Employees`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the employee tolerance group maintenance activity.
2. Select the required Tolerance Group.
3. Enter the user name in the User Name field.
4. Verify the selected tolerance group and user assignment.
5. Confirm that the intended posting limits apply.
6. Save the assignment.

## 5. Assignment Record

| Field | Project value |
|---|---|
| Tolerance Group | To be recorded from SAP |
| User Name | Use a redacted or non-personal example in the public portfolio |
| Assignment result | Pending verification |

## 6. Validation

- [ ] Tolerance Group exists.
- [ ] User assignment is maintained.
- [ ] Correct tolerance group is assigned to the intended user.
- [ ] Applicable posting limits are checked.
- [ ] Assignment can be displayed after saving.

## 7. Evidence

Suggested screenshot: `07-Assign-User-Tolerance-Group.png`

Redact personal user IDs and any sensitive authorization information before publishing.

## 8. Implementation Notes

The source document's navigation points to the employee tolerance group activity. Record the exact screen and assignment method used in the project system.

## 9. Source Note

Based on Phase 2, section 2.4.1, Assign User Name to Tolerance Group for Employees, in the uploaded SAP FICO implementation project document.
