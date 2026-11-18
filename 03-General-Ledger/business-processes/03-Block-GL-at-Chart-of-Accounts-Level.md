# Process 3: Block G/L at Chart of Accounts Level for Posting – Loan Account

## 1. Objective

Document the blocking of a G/L account for posting at the Chart of Accounts level.

## 2. Business Purpose

The source describes this control as restricting postings to a G/L account across company codes that use the same Chart of Accounts. Its example is a Loan Account that should not accept unauthorized or incorrect postings.

## 3. Process Flow

- Preceding process: G/L Master Data
- Required process: Block G/L Master Data
- Succeeding process: Unblock G/L Master Data

## 4. Prerequisites

- Configuration required: Nil, according to the source.
- Master data required: G/L Master — Loan Account.
- Transaction code stated in source: `FS00`.

## 5. Procedure Outline

1. Display the Loan G/L account in the G/L master maintenance activity.
2. Navigate to the Chart of Accounts segment.
3. Apply the posting block described in the project procedure.
4. Save the change.
5. Verify that the account displays the posting block.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] The Chart of Accounts-level block is visible in the master record.
- [ ] The block applies at the intended level.
- [ ] Posting restriction is validated in a controlled test, if performed.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.29](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=29). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

## 8. Source Note

Business Processes document, Process 3, pages 28–29.