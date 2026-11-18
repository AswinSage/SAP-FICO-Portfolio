# Assign Company Code to Company

## 1. Objective

Document the organizational assignment linking the company code to the company defined in the Enterprise Structure.

## 2. Business Purpose

The assignment establishes the relationship between the accounting entity and the company-level organizational structure used in the project.

## 3. Configuration Activity

**Configuration item:** Assign Company Code to Company

**Configuration area:** Enterprise Structure

**SAP navigation:** Record the exact IMG/SPRO path used in the project system.

**Transaction code:** Record the transaction code actually used. Do not infer it.

## 4. Procedure Record

1. Open the Enterprise Structure assignment activity.
2. Locate the company code created for the project.
3. Assign it to the appropriate company defined in the project design.
4. Review the selected company and company code identifiers.
5. Save the assignment.
6. Re-open the assignment view and verify the relationship.

## 5. Assignment Record

| Field | Project value |
|---|---|
| Company Code | To be entered from project evidence |
| Company | To be entered from project evidence |
| Assignment result | Pending evidence |

## 6. Validation

- [ ] Company exists.
- [ ] Company code exists.
- [ ] Company code is assigned to the intended company.
- [ ] Assignment is saved and can be displayed.
- [ ] Screenshot or configuration export is available.

## 7. Evidence

Suggested filename: `03-Assign-Company-Code-to-Company.png`

## 8. Source Note

The uploaded implementation project document lists the company code-to-company assignment as an Enterprise Structure activity. The actual identifiers and successful execution must be confirmed from the project system.
