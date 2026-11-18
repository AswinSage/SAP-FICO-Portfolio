# Process 1: Create G/L Master Data

## 1. Objective

Create G/L master records required to classify and record financial transactions.

## 2. Business Purpose

The source describes G/L master data as the foundation for financial postings. Each account is connected to a Chart of Accounts and assigned to a company code. Account settings govern posting rules, currency, field status, and tax-related settings.

## 3. Process Flow

- Preceding process: Nil
- Required process: G/L Master Creation
- Succeeding process: G/L Posting

## 4. Prerequisites

**Configuration required**
- Chart of Accounts
- Account Group
- Field Status Variant
- Retained Earnings Account
- Tolerance Group for G/L

**Master data / transaction**
- G/L Master Data

**Transaction code stated in source:** `FS00`

## 5. Procedure Outline

1. Open G/L account master maintenance using the transaction stated in the source.
2. Create the required G/L account records for the project.
3. Maintain the applicable Chart of Accounts and company code information.
4. Maintain account classification and relevant control settings.
5. Save and verify each account.

The source includes examples for Cash, Sundry Debtors, Furniture, Plant & Machinery, Loan, Capital, Sundry Creditors, Bank Overdraft, Rent, Telephone Charges, Audit Fees, Maintenance Charges, Cash Discount Received, Sales Account, Interest Received, and Commission Received. Capture only the accounts actually created in the project.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] Required G/L accounts can be displayed.
- [ ] Account descriptions and classifications are checked.
- [ ] Company code assignments and control settings are verified.
- [ ] G/L line-item report can be executed for relevant accounts.

## 7. Evidence

Suggested evidence: `01-Create-GL-Master-Data.png` and redacted account display screenshots.

## 8. Implementation Notes

Record actual G/L numbers, descriptions, account groups, and account types from the project system. Do not publish confidential account information.

## 9. Source Note

Business Processes document, Process 1, pages 1–25. The source names `FS00` for G/L master creation.