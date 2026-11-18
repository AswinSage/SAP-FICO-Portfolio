# Process 17: Customer Invoice

## 1. Objective

Document posting of a customer invoice for services provided.

## 2. Business Purpose

The source describes customer invoice posting as recognition of a receivable from the customer and corresponding revenue. The posting automatically updates the customer reconciliation account in the General Ledger.

## 3. Process Flow

- Preceding process: Customer Master Data and G/L Master Data
- Required process: Customer Invoice
- Succeeding process: Customer Payment

## 4. Prerequisites

**Configuration required**
- Document Type
- Number Range
- Posting Period Variant
- Posting Key
- Tolerance Group for Employees

**Master data**
- Customer Master (`XD01`)
- G/L Master (`FS00`)

## 5. Procedure Outline

1. Confirm the customer master and revenue G/L account are available.
2. Confirm the posting period is open.
3. Open the customer invoice posting activity used in the project.
4. Enter customer, invoice date, posting date, reference, and amount as applicable.
5. Enter the corresponding revenue line and other required details.
6. Verify debit and credit totals.
7. Post the invoice and record the generated document number.
8. Verify the customer open item and G/L posting.

The source example is a service invoice to Unisoft Infotech Pvt Ltd.

## 6. Validation and Reporting

**Reports stated in source**
- Customer Line-item Report — `FBL5N`
- G/L Line-item Report — `FBL3N`

- [ ] Customer receivable is recorded.
- [ ] Revenue is recorded.
- [ ] Customer reconciliation account is updated.
- [ ] Invoice appears in customer line items.
- [ ] Revenue appears in G/L line items.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.62](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=62) · [PDF p.63](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=63) · [PDF p.64](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=64) · [PDF p.65](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=65). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`17-Customer-Service-Invoice.png`, plus customer and G/L line-item reports.

## 8. Implementation Notes

Record actual customer, revenue account, invoice reference, date, amount, and document number only if safe to disclose.

## 9. Source Note

Business Processes document, Process 17, pages 62–64.