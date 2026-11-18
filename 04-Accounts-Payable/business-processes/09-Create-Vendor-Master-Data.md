# Process 9: Create Vendor Master Data

## 1. Objective

Document creation of vendor master records for suppliers providing goods or services.

## 2. Business Purpose

The source describes vendor master data as containing general and company code information, together with purchasing information referenced by the source. It is used for supplier-related invoice postings and payments.

## 3. Process Flow

- Preceding process: Nil
- Required process: Vendor Master Data
- Succeeding process: Posting (Invoice, G/L, Special G/L Transaction)

## 4. Prerequisites

**Configuration required**
- Account Group for Vendors
- Number Range for Vendors
- Tolerance Group for Vendors
- Payment Terms

**Master data**
- Vendor Master Creation (`XK01`)
- G/L Master (`FS00`) — Vendor Reconciliation Account

## 5. Procedure Outline

1. Open vendor master creation using the transaction stated in the source.
2. Enter the vendor account group and required organizational data.
3. Maintain the vendor's general data.
4. Maintain company code data and relevant payment details.
5. Enter the vendor reconciliation account and payment terms as required.
6. Save the vendor master record.
7. Display the record and verify the maintained data.

The source examples include BE Solution Pvt Ltd and Sun IT Solutions. Use these names only if they are approved for public disclosure; otherwise replace them with redacted labels.

## 6. Validation and Reporting

**Report stated in source:** Vendor Line-item Report — `FBL1N`

- [ ] Vendor master record is created.
- [ ] Account group and number range are correct.
- [ ] Company code data is maintained.
- [ ] Reconciliation account and payment terms are checked.
- [ ] Vendor can be selected for subsequent postings.

## 7. Evidence

Suggested evidence: `09-Create-Vendor-Master.png`.

## 8. Implementation Notes

Record actual account group, vendor number, company code, reconciliation account, and payment terms. Redact supplier personal or confidential details before publication.

## 9. Source Note

Business Processes document, Process 9, pages 39–42.