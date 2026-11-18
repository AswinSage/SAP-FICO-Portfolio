# Define Company

## 1. Objective

Define the company-level organizational unit required by the Enterprise Structure design.

## 2. Business Purpose

A company represents a corporate entity in the organizational structure. In the project design, this activity forms part of the foundation for assigning the company code and supporting group-level organizational representation.

## 3. Configuration Activity

**Configuration item:** Define Company

**Configuration area:** Enterprise Structure

**SAP navigation:** Use the relevant Enterprise Structure definition activity in the IMG/SPRO structure available in the project system. Record the exact menu path used during execution.

**Transaction code:** Record the code actually used in the project system. Do not infer it from a generic procedure.

## 4. Procedure Record

1. Open the Enterprise Structure configuration area.
2. Select the activity to define a company.
3. Create or maintain the company entry according to the approved project design.
4. Enter the required organizational details.
5. Save the configuration.
6. Re-open or display the entry to verify that it was saved.

## 5. Project Configuration Values

| Field | Value visible in SRC-01 | Source |
|---|---|---|
| Company ID | HM11 | PDF page 2 |
| Company name | Hindustan Motors Ltd | PDF pages 2 and 4 |
| Street / House number | Ferry Street / 122 | PDF page 4 |
| City | Chennai | PDF pages 2 and 4 |
| Postal Code / PO Box | 600122 / 600122 | PDF pages 2 and 4 |
| Country / Region | IN / 22 | PDF page 4 |
| Language / Currency | EN / INR | PDF pages 2 and 4 |

These are values visible in the supplied implementation report. Reconfirm them in the target SAP tenant before reuse.

## 6. Validation

- [ ] Company entry exists in the configuration system.
- [ ] Company identifier matches the approved project design.
- [ ] Company description is correct.
- [ ] Saved configuration can be displayed again.
- [ ] Evidence screenshot is available and redacted.

## 7. Evidence

Add a redacted screenshot showing the company definition and saved entry.

Suggested filename: `01-Define-Company.png`

## 8. Implementation Notes

Capture any issue, decision, or correction made during the actual project execution. Leave this section marked as pending until the real system details have been added.

## 9. Source Note

The uploaded SAP FICO implementation project document includes Define Company as an Enterprise Structure activity. The field values and exact execution details must be taken from the project's own system evidence.
