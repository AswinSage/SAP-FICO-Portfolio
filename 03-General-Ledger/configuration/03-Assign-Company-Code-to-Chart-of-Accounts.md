# Assign Company Code to Chart of Accounts

## 1. Objective

Document the assignment of a company code to the Chart of Accounts used for its G/L accounting structure.

## 2. Business Purpose

The assignment determines which Chart of Accounts provides the G/L account definitions available to the company code. The source project describes this relationship as supporting consistent G/L account management and financial reporting.

## 3. Configuration Activity

**Configuration item:** Assign Company Code to Chart of Accounts

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Ledgers → Master Data → G/L Accounts → Preparations → Assign Company Code to Chart of Accounts`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Assign Company Code to Chart of Accounts activity.
2. Select the required company code.
3. Enter the Chart of Accounts.
4. Verify the assignment.
5. Save the configuration.

## 5. Assignment Record

| Field | Project value |
|---|---|
| Company Code | HM11 is defined in SRC-01, PDF page 4 |
| Chart of Accounts | HM11 is defined in SRC-01, PDF page 29 |
| Assignment result | The PDF describes the assignment procedure but does not show a saved assignment result. Verify the company-code assignment in the target system. |

## 6. Validation

- [ ] Company code exists.
- [ ] Chart of Accounts exists.
- [ ] Correct Chart of Accounts is assigned to the company code.
- [ ] Assignment is saved and can be displayed.

## 7. Evidence

Suggested screenshot: `02-Assign-Company-Code-to-Chart-of-Accounts.png`

## 8. Implementation Notes

Record the actual company code and Chart of Accounts identifiers from the SAP project system.

## 9. Source Note

Based on Phase 3, section 3.1.1, Assign Company Code to Chart of Accounts, in the uploaded SAP FICO implementation project document.
