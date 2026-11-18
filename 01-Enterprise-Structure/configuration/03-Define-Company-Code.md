# Define Company Code

## 1. Objective

Document the definition of the company code used as the accounting organizational unit in the SAP FICO project.

## 2. Business Purpose

The company code is the organizational level at which the project maintains financial accounting records and prepares company-code financial statements.

## 3. Configuration Activity

**Configuration item:** Define Company Code

**Configuration area:** Enterprise Structure

**SAP navigation:** Record the exact IMG/SPRO path used in the project system.

**Transaction code:** Record the transaction code actually used. Do not add an unverified code.

## 4. Procedure Record

1. Access the Enterprise Structure configuration area.
2. Select the company code definition activity.
3. Create or maintain the company code according to the approved project design.
4. Enter the required company code attributes.
5. Save the entry.
6. Display the saved company code and verify the values.

## 5. Project Configuration Values

| Field | Value visible in SRC-01 | Source |
|---|---|---|
| Company Code | HM11 | PDF page 4 |
| Company Code Name | Hindustan Motors Ltd | PDF page 4 |
| City | Chennai | PDF page 4 |
| Country / Region | IN / 22 | PDF page 4 |
| Currency | INR | PDF page 4 |
| Language | EN | PDF page 4 |
| Street / House number | Ferry Street / 122 | PDF page 4 |
| Postal Code / PO Box | 600122 / 600122 | PDF page 4 |

These values are transcribed from the project report screenshot and are not a substitute for checking the target SAP configuration.

## 6. Validation

- [ ] Company code has been created or maintained.
- [ ] Identifier and description match the project design.
- [ ] Country and currency values have been checked.
- [ ] Saved values can be displayed.
- [ ] Required relationships to other organizational units are documented.
- [ ] Redacted screenshot is available.

## 7. Evidence

Suggested filename: `02-Define-Company-Code.png`

## 8. Implementation Notes

Record the actual values, system messages, and any configuration issues encountered during execution. Do not mark the activity complete without evidence.

## 9. Source Note

Define Company Code is listed in the Enterprise Structure phase of the uploaded implementation project document. Populate project-specific values from the SAP system evidence, not assumptions.
