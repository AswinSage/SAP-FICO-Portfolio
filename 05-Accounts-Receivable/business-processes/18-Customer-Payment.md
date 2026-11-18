# Process 18: Customer Payment

## 1. Objective

Document receipt of customer payment against an outstanding invoice.

## 2. Business Purpose

The source describes customer payment as clearing an outstanding receivable and updating the bank or cash account. It identifies full, partial, and residual payment as possible payment outcomes.

## 3. Process Flow

- Preceding process: Customer Invoice
- Required process: Customer Payment
- Succeeding process: Customer Line-item Report

## 4. Prerequisites

**Configuration required**
- Document Type
- Number Range
- Posting Period Variant
- Posting Key
- Tolerance Group for Employees
- Tolerance Group for Customers

**Master data**
- Customer Master (`XD01`)
- G/L Master (`FS00`)

## 5. Procedure Outline

1. Identify the outstanding customer invoice.
2. Confirm the customer account and relevant bank or cash G/L account.
3. Open the customer payment activity used in the project.
4. Enter the payment details and select the invoice or open item.
5. Process the full, partial, or residual payment scenario performed in the project.
6. Review the clearing status and any remaining open balance.
7. Post the payment and record the generated document number.
8. Verify customer and G/L account updates.

## 6. Validation and Reporting

**Reports stated in source**
- Customer Line-item Report — `FBL5N`
- G/L Line-item Report — `FBL3N`

- [ ] Payment document is posted.
- [ ] Customer open item is cleared or partially open as expected.
- [ ] Bank or cash account is updated.
- [ ] Customer and G/L reports reflect the payment.

## 7. Evidence

Suggested evidence: `18-Customer-Payment.png` and related line-item reports.

## 8. Implementation Notes

Record which payment scenario was actually performed. Do not claim full, partial, and residual scenarios were all tested without separate evidence.

## 9. Source Note

Business Processes document, Process 18, pages 65–67.