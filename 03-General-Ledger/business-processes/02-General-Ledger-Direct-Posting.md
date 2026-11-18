# Process 2: General Ledger Posting – Direct

## 1. Objective

Document direct posting of business expenses to General Ledger accounts without using customer or vendor sub-ledger accounts.

## 2. Business Purpose

The source describes direct G/L posting for day-to-day expenses such as rent, telephone charges, electricity, and office expenses. The expense account and cash or bank account are updated through the posting.

## 3. Process Flow

- Preceding process: G/L Master Creation
- Required process: G/L Posting
- Succeeding process: G/L Line-item Report

## 4. Prerequisites

**Configuration required**
- Document Type
- Number Range
- Posting Period Variant
- Posting Key
- Tolerance Group for Employees

**Master data**
- G/L Master Data (`FS00`)


## 5. Procedure Outline

1. Confirm that the relevant expense and cash/bank G/L accounts exist.
2. Confirm that the posting period is open.
3. Enter the direct expense posting using the transaction actually used in the project system.
4. Enter the relevant document header and debit/credit line items.
5. Check amounts, posting dates, account assignments, and balancing.
6. Post the document and record the generated document number.

The source illustrates Rent Paid and Telephone Charges Paid postings.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] Posted document is displayed.
- [ ] Expense and cash/bank entries are reflected in the correct accounts.
- [ ] Debit and credit totals balance.
- [ ] Line-item report reflects the posting.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.27](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=27). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

## 8. Source Note

Business Processes document, Process 2, pages 26–27. The source lists the prerequisite configuration and examples of rent and telephone postings.