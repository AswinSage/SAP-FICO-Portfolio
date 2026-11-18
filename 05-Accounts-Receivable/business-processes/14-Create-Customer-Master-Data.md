# Process 14: Create Customer Master Data

## 1. Objective

Document creation of customer master records used for customer invoices, incoming payments, and reporting.

## 2. Business Purpose

The source describes customer master data as containing general data, company code data, and sales area data. It provides the customer information required for accounting and sales transactions.

## 3. Process Flow

- Preceding process: Nil
- Required process: Customer Master Data
- Succeeding process: Customer Posting (Invoice, Posting, Special G/L Transactions)

## 4. Prerequisites

**Configuration required**
- Account Group for Customers
- Number Range for Customers
- Tolerance Group for Customers
- Payment Terms

**Master data**
- Customer Master (`XD01`)
- G/L Master (`FS00`)

## 5. Procedure Outline

1. Open customer master creation using the transaction stated in the source.
2. Select the customer account group.
3. Maintain general customer data.
4. Maintain company code data.
5. Maintain sales area data if required by the project scenario.
6. Enter reconciliation account and payment terms as applicable.
7. Save and display the customer master record.

The source examples include Unisoft Infotech Pvt Ltd and Zyple Software Solutions Pvt Ltd. Confirm authorization before publishing customer names.

## 6. Validation and Reporting

**Report stated in source:** Customer Line-item Report — `FBL5N`

- [ ] Customer master record is created.
- [ ] Account group and number range are correct.
- [ ] Company code data is maintained.
- [ ] Reconciliation account and payment terms are checked.
- [ ] Customer can be selected for subsequent postings.

## 7. Evidence

**Source PDF screenshot pages:** 54-57 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`14-Create-Customer-Master.png`.

## 8. Implementation Notes

Record actual customer account group, company code, reconciliation account, and payment terms. Redact personal or confidential customer information.

## 9. Source Note

Business Processes document, Process 14, pages 53–57.