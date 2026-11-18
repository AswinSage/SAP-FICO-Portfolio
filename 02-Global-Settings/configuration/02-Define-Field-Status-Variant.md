# Define Field Status Variant

## 1. Objective

Define a Field Status Variant to control how G/L account fields behave during financial document entry.

## 2. Business Purpose

The Field Status Variant controls whether fields are required, optional, suppressed, or display-only during posting. It contains Field Status Groups used for different G/L accounts and helps standardize the information collected during financial transactions.

## 3. Configuration Activity

**Configuration item:** Define Field Status Variants

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Document → Line Item → Controls → Define Field Status Variants`

**Transaction code:** Not specified in the source procedure. Record the code actually used in the project system, if applicable.

## 4. Procedure

1. Open the Define Field Status Variants activity.
2. Select **New Entries**.
3. Enter the four-character Field Status Variant.
4. Enter the description.
5. Save the Field Status Variant.
6. Select the created variant.
7. Open **Field Status Groups**.
8. Select **New Entries**.
9. Enter the Field Status Group and description.
10. Maintain the required field status settings.
11. Save the Field Status Group entries.

## 5. Project Configuration Values

| Field | Project value |
|---|---|
| Field Status Variant | To be recorded from SAP |
| Description | To be recorded from SAP |
| Field Status Group | To be recorded from SAP |
| Field Status Group description | To be recorded from SAP |
| Field control settings | To be recorded from SAP |

## 6. Validation

- [ ] Four-character variant identifier is maintained.
- [ ] Description is correct.
- [ ] Required Field Status Groups are created.
- [ ] Field control settings match the project requirement.
- [ ] Configuration can be displayed after saving.

## 7. Evidence

Suggested screenshot: `01-Define-Field-Status-Variant.png`

Capture the variant and its Field Status Groups. Redact sensitive system information.

## 8. Implementation Notes

Record any field-control decisions and issues encountered during execution. Do not assume a field is required or suppressed unless the actual configuration confirms it.

## 9. Source Note

Based on Phase 2, section 2.1, Field Status Variant, in the uploaded SAP FICO implementation project document.
