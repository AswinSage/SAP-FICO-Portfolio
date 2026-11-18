# Assign Company Code to Field Status Variant

## 1. Objective

Document the assignment of a Field Status Variant to the relevant company code.

## 2. Business Purpose

The assignment determines the field status controls applied during G/L account postings for the company code. The Field Status Variant contains Field Status Groups that define field behavior during financial document entry.

## 3. Configuration Activity

**Configuration item:** Assign Company Code to Field Status Variant

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Ledgers → Fields → Assign Company Code to Field Status Variant`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the company code assignment activity.
2. Select the required company code.
3. Enter the Field Status Variant.
4. Verify the company code and variant relationship.
5. Save the assignment.

## 5. Assignment Record

| Field | Project value |
|---|---|
| Company Code | HM11 is defined in SRC-01, PDF page 4 |
| Field Status Variant | HM11 is defined in SRC-01, PDF page 20 |

## 6. Validation

- [ ] Company code exists.
- [ ] Field Status Variant exists.
- [ ] Correct variant is assigned to the intended company code.
- [ ] Assignment can be displayed after saving.

## 7. Evidence

Suggested screenshot: `02-Assign-Field-Status-Variant.png`

## 8. Implementation Notes

Record the actual company code, variant, and any issues encountered. Do not publish confidential organizational identifiers without authorization.

## 9. Source Note

Based on Phase 2, section 2.1.1, Assign Company Code to Field Status Variant, in the uploaded implementation project document.
