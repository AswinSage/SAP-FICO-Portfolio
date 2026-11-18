# Process 19: Customer Line-item Report

## 1. Objective

Document review of all transactions posted to a customer account.

## 2. Business Purpose

The source describes the Customer Line-item Report as displaying invoices, incoming payments, credit memos, clearing documents, and outstanding balances. It supports monitoring receivables, open items, cleared items, and customer payment history.

## 3. Process Flow

- Preceding process: Customer Posting
- Required process: Customer Line-item Report
- Succeeding process: Nil

## 4. Prerequisites

- Configuration required: Nil, according to the source.
- Master data required: Customer Master Data (`XD01`).
- Report stated in source: `FBL5N`.

## 5. Procedure Outline

1. Open the Customer Line-item Report.
2. Enter the customer account and company code.
3. Select the required date range and open/cleared item criteria.
4. Execute the report.
5. Review invoices, incoming payments, clearing documents, and outstanding balances.
6. Capture the report output.

## 6. Validation

- [ ] Correct customer and company code are selected.
- [ ] Relevant invoice and payment entries are displayed.
- [ ] Open and cleared item status is reviewed.
- [ ] Report agrees with the related posting documents.

## 7. Evidence

**Source PDF screenshot pages:** 69 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`19-Customer-Line-Item-Report.png`.

## 8. Implementation Notes

The source's final report list includes `FS00` next to the G/L Line-item Report label. This appears inconsistent with the report transaction reference used elsewhere in the same document (`FBL3N)). Verify the actual report transaction from the project evidence before publishing it as the G/L report code.

## 9. Source Note

Business Processes document, Process 19, pages 68–69.