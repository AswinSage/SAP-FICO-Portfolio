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

**Source PDF screenshot pages:** [PDF p.2](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=2) · [PDF p.3](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=3) · [PDF p.4](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=4) · [PDF p.5](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=5) · [PDF p.6](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=6) · [PDF p.7](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=7) · [PDF p.8](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=8) · [PDF p.9](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=9) · [PDF p.10](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=10) · [PDF p.11](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=11) · [PDF p.12](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=12) · [PDF p.13](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=13) · [PDF p.14](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=14) · [PDF p.15](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=15) · [PDF p.16](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=16) · [PDF p.17](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=17) · [PDF p.18](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=18) · [PDF p.19](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=19) · [PDF p.20](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=20) · [PDF p.21](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=21) · [PDF p.22](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=22) · [PDF p.23](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=23) · [PDF p.24](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=24) · [PDF p.25](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=25). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

## 8. Source Note

Business Processes document, Process 1, pages 1–25. The source names `FS00` for G/L master creation.