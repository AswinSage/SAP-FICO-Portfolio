# Process 11: Vendor Invoice – Rent Invoice of BE Solution Pvt Ltd

## 1. Objective

Document posting of a rent invoice received from the vendor identified in the source process.

## 2. Business Purpose

The source describes vendor invoice posting as recognition of a liability to the vendor and the corresponding rent expense. The posting also updates the vendor reconciliation account in the General Ledger.

## 3. Process Flow

- Preceding process: Vendor Master Data and G/L Master Data
- Required process: Vendor Invoice Creation
- Succeeding process: Vendor Payment

## 4. Prerequisites

**Configuration required**
- Document Type
- Number Range
- Posting Period Variant
- Posting Key
- Tolerance Group for Employees

**Master data**
- Vendor Master (`XK01`)
- G/L Master (`FS00`)

## 5. Procedure Outline

1. Confirm that the vendor master and relevant rent expense G/L account exist.
2. Confirm that the posting period is open.
3. Open the vendor invoice posting activity used in the project.
4. Enter the vendor, invoice date, posting date, reference, and amount as applicable.
5. Enter the rent expense line and relevant tax or other details only if they are part of the actual project case.
6. Check debit and credit totals.
7. Post the invoice and record the generated document number.
8. Verify the vendor open item and expense posting.

The source identifies the invoice as a rent invoice for BE Solution Pvt Ltd.

## 6. Validation and Reporting

**Reports stated in source**
- Vendor Line-item Report — `FBL1N`
- G/L Line-item Report — `FBL3N`

- [ ] Vendor liability is recorded.
- [ ] Rent expense is recorded.
- [ ] Vendor reconciliation account is updated.
- [ ] Invoice appears in the vendor line-item report.
- [ ] Expense appears in the G/L line-item report.

## 7. Evidence

**Source PDF screenshot pages:** 48-49 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`11-Vendor-Rent-Invoice.png`, plus vendor and G/L line-item reports.

## 8. Implementation Notes

Record the actual invoice reference, posting date, amount, vendor account, expense account, and document number only if safe for public release. Do not invent invoice values.

## 9. Source Note

Business Processes document, Process 11, pages 47–48.