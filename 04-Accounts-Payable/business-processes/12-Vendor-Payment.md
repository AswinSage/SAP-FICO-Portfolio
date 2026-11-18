# Process 12: Vendor Payment

## 1. Objective

Document payment of an outstanding vendor invoice, including the partial payment and residual payment concepts described in the source.

## 2. Business Purpose

The source distinguishes:
- Partial payment: only part of the invoice amount is paid, while the original invoice remains open for the balance.
- Residual payment: the original invoice is cleared and the remaining balance is transferred to a new open item.

These approaches support vendor liability and cash-flow management.

## 3. Process Flow

- Preceding process: Vendor Invoice
- Required process: Vendor Payment
- Succeeding process: Vendor Line-item Report

## 4. Prerequisites

**Configuration required**
- Document Type
- Number Range
- Posting Period Variant
- Tolerance Group for Vendors
- Tolerance Group for Employees
- Posting Key

**Master data**
- G/L Master Data (`FS00`)
- Vendor Master Data (`XK01`)

## 5. Procedure Outline

1. Identify the outstanding vendor invoice.
2. Confirm the vendor account and relevant cash/bank G/L account.
3. Open the vendor payment activity used in the project.
4. Enter the payment details and select the outstanding invoice.
5. Process the partial payment or residual payment scenario as applicable.
6. Review the clearing and remaining open-item result.
7. Post the payment and record the generated document number.
8. Verify the vendor account.

## 6. Validation and Reporting

**Reports stated in source**
- Vendor Line-item Report — `FBL1N`
- G/L Line-item Report — `FBL3N`

- [ ] Payment document is posted.
- [ ] Partial payment leaves the original invoice open for the remaining amount, where tested.
- [ ] Residual payment clears the original item and creates the residual open item, where tested.
- [ ] Vendor and G/L reports reflect the payment.

## 7. Evidence

Suggested evidence: `12-Vendor-Payment-Partial.png` and `12-Vendor-Payment-Residual.png`.

## 8. Implementation Notes

The source includes both partial and residual payment examples. Record the actual scenario performed and the resulting open-item status. Do not claim both were tested unless both have evidence.

## 9. Source Note

Business Processes document, Process 12, pages 49–51.