# Assign Fiscal Year Variant to Company Code

## 1. Objective

Document the assignment of the required Fiscal Year Variant to a company code.

## 2. Business Purpose

The assignment establishes the accounting calendar used by the company code. It controls the posting periods and special periods used to classify transaction posting dates for financial accounting and reporting.

## 3. Configuration Activity

**Configuration item:** Assign Company Code to a Fiscal Year Variant

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Ledgers → Fiscal Year and Posting Periods → Assign Company Code to a Fiscal Year Variant`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the company code assignment activity.
2. Select the required company code.
3. Enter the Fiscal Year Variant.
4. Verify the assigned variant.
5. Save the assignment.

## 5. Assignment Record

| Field | Project value |
|---|---|
| Company Code | HM11 is defined in SRC-01, PDF page 4 |
| Fiscal Year Variant | HM (Jan-Dec) is defined in SRC-01, PDF page 23 |
| Assignment result | The PDF describes the assignment procedure but does not show a saved assignment result. Verify the company-code assignment in the target system. |

## 6. Validation

- [ ] Company code exists.
- [ ] Fiscal Year Variant exists.
- [ ] Correct variant is assigned to the company code.
- [ ] Assignment is saved and can be displayed.
- [ ] Period structure is consistent with the approved project design.

## 7. Evidence

Suggested screenshot: `04-Assign-Fiscal-Year-Variant.png`

## 8. Implementation Notes

Record the company code and assigned variant from the actual project system.

## 9. Source Note

Based on Phase 2, section 2.2.1, Assign Fiscal Year Variant to Company Code, in the uploaded implementation project document.
