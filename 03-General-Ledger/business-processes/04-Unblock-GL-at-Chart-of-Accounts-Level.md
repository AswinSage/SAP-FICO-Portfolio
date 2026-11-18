# Process 4: Unblock G/L at Chart of Accounts Level for Posting – Loan Account

## 1. Objective

Document removal of a posting block maintained at the Chart of Accounts level.

## 2. Business Purpose

The source describes unblocking as the action taken when a previously restricted G/L account, such as the Loan Account example, needs to be activated for financial transactions again.

## 3. Process Flow

- Preceding process: Block G/L Master Data
- Required process: Unblock G/L Master Data
- Succeeding process: Posting

## 4. Prerequisites

- Configuration required: Nil, according to the source.
- Master data required: G/L Master — Loan Account.
- Transaction code stated in source: `FS00`.

## 5. Procedure Outline

1. Display the Loan G/L account in master maintenance.
2. Navigate to the Chart of Accounts segment.
3. Remove the posting block applied in Process 3.
4. Save the change.
5. Display the account again and verify that the block has been removed.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] The Chart of Accounts-level block is no longer active.
- [ ] The master record reflects the updated status.
- [ ] A controlled posting test is recorded if performed.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.31](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=31). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

## 8. Source Note

Business Processes document, Process 4, pages 30–31.