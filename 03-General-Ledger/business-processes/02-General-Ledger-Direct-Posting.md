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

**Source transaction-code note:** The source text says that G/L posting can be made using `FS00`. This appears inconsistent with its own identification of `FS00` as G/L master maintenance in Process 1. Verify the actual posting transaction used in the SAP project system before publishing a transaction code for posting.

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

**Source PDF screenshot pages:** 27 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`02-Direct-GL-Posting-Rent.png`, `02-Direct-GL-Posting-Telephone.png`, and relevant redacted report output.

## 8. Implementation Notes

Record the actual transaction code used, document type, posting date, G/L accounts, and validation result. Do not copy the source's `FS00` posting reference without checking the project evidence.

## 9. Source Note

Business Processes document, Process 2, pages 26–27. The source lists the prerequisite configuration and examples of rent and telephone postings.