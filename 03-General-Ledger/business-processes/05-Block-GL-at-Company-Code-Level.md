# Process 5: Block G/L at Company Code Level for Creation and Posting – Loan Account

## 1. Objective

Document blocking of a G/L account at the company code level for creation and posting.

## 2. Business Purpose

The source describes this control as restricting use of a G/L account within a specific company code. The example is a Loan Account that should not be used for further transactions in the selected company code.

## 3. Process Flow

- Preceding process: G/L Master Data
- Required process: Block G/L Master Data
- Succeeding process: Unblock G/L Master Data

## 4. Prerequisites

- Configuration required: Nil, according to the source.
- Master data required: G/L Master Data.
- Transaction code stated in source: `FS00`.

## 5. Procedure Outline

1. Open the G/L master record for the Loan Account.
2. Select the relevant company code segment.
3. Apply the company code-level block for creation and posting as described in the project system.
4. Save the change.
5. Display the company code segment and verify the block.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] The block is maintained at company code level.
- [ ] The selected company code is correct.
- [ ] The updated master record can be displayed.
- [ ] Posting restriction test result is recorded if performed.

## 7. Evidence

**Source PDF screenshot pages:** 32 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`05-Block-GL-Company-Code-Level.png`.

## 8. Implementation Notes

Do not confuse a company code-level block with a Chart of Accounts-level block. Record the exact block scope shown in the SAP system.

## 9. Source Note

Business Processes document, Process 5, pages 31–32.