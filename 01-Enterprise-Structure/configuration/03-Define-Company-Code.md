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

| Field | Project value | Notes |
|---|---|---|
| Company Code | To be entered from project evidence | Do not invent |
| Company Code Name | To be entered from project evidence | Use approved project wording |
| Country / region | To be entered from project evidence | Verify against system |
| Currency | To be entered from project evidence | Verify against system |
| Additional attributes | As shown in SAP evidence | Include only relevant fields |

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
