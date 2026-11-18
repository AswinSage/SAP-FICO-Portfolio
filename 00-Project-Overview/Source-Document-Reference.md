# Source Document Reference and Project Configuration Snapshot

## 1. Purpose

This document records the project-specific information visible in the two supplied SAP FICO PDFs. It links the source material to the portfolio sections and separates values that are visible in the PDFs from items that still require live-system verification.

**Important:** The values below are transcribed from the supplied source report and its embedded SAP screenshots. They are not a claim that the same configuration has been recreated or validated in a current SAP S/4HANA Private Cloud tenant.

## 2. Source Document Register

| Source ID | Source document | Length | Coverage |
|---|---|---:|---|
| SRC-01 | SAP FICO Implementation Project for Hindustan Motors Ltd | 155 PDF pages | Eight implementation phases covering Enterprise Structure, Global Settings, G/L, AP, AR, Asset Accounting, Controlling, and cutover/testing |
| SRC-02 | Business Process for SAP FICO | 92 PDF pages | 27 numbered processes covering G/L, AP, AR, Asset Accounting, and CO |

The repository contains structured Markdown documentation derived from these documents. The original PDFs themselves are not stored in this GitHub repository.

## 3. Project Identity and Enterprise Structure

The implementation report identifies the case as **Hindustan Motors Ltd**.

| Field | Value visible in source | Source location |
|---|---|---|
| Company ID | HM11 | SRC-01, PDF page 2 |
| Company name | Hindustan Motors Ltd | SRC-01, PDF pages 2 and 4 |
| Company Code | HM11 | SRC-01, PDF page 4 |
| City | Chennai | SRC-01, PDF pages 2 and 4 |
| Street / House number | Ferry Street / 122 | SRC-01, PDF page 4 |
| Postal Code | 600122 | SRC-01, PDF page 4 |
| PO Box | 600122 | SRC-01, PDF page 4 |
| Country | IN | SRC-01, PDF page 4 |
| Region | 22 | SRC-01, PDF page 4 |
| Language | EN | SRC-01, PDF pages 2 and 4 |
| Local currency | INR | SRC-01, PDF pages 2 and 4 |

### Credit Control Area

| Field | Value visible in source |
|---|---|
| Credit Control Area | HM11 |
| Description | Credit Control Area - HM11 |
| Currency | INR |
| Fiscal Year Variant field | H1 |
| Credit Limit | 1,500,000,000 |

Source: SRC-01, PDF page 7. The Update setting is not transcribed here because the screenshot does not provide a sufficiently clear value.

## 4. Global Settings Snapshot

| Configuration item | Value visible in source | Source location |
|---|---|---|
| Field Status Variant | HM11 | SRC-01, PDF page 20 |
| Field Status Variant description | Field Status Variant-HM11 | SRC-01, PDF page 20 |
| Fiscal Year Variant | HM | SRC-01, PDF page 23 |
| Fiscal Year description | Jan-Dec | SRC-01, PDF page 23 |
| Calendar year indicator | Selected | SRC-01, PDF page 23 |
| Posting periods | 12 | SRC-01, PDF page 23 |
| Special periods | 4 | SRC-01, PDF page 23 |

The source screenshot shows multiple fiscal-year variants. The values above refer specifically to the row labelled HM.

## 5. General Ledger Snapshot

### Chart of Accounts

| Field | Value visible in source |
|---|---|
| Chart of Accounts | HM11 |
| Description | Chart of Accounts - HM11 |
| Maintenance language | EN |
| G/L account number length | 6 |
| Controlling integration | Manual creation of cost elements |

Source: SRC-01, PDF page 29.

### Retained Earnings Assignment

| Field | Value visible in source |
|---|---|
| Chart of Accounts | HM11 |
| P&L statement account type | BIL |
| Retained Earnings Account | 1000 |

Source: SRC-01, PDF page 33.

### Sample G/L Master Records

The following records are examples displayed in the source screenshots. The account numbers are preserved as shown; confirm them in the live project system before reuse.

| G/L account | Company Code | Short / long description | Account Group | Account type | Source location |
|---:|---|---|---|---|---|
| 1 | HM11 | Machine | AST ASSET | Balance Sheet | SRC-01, PDF page 35 |
| 2 | HM11 | Cash Account | AST ASSET | Balance Sheet | SRC-01, PDF page 37 |
| 1001 | HM11 | Loan / Loan Account | LIAB LIABILITY | Balance Sheet | SRC-01, PDF page 39 |
| 2001 | HM11 | Rent Account | EXP EXPENSES | P&L Statement | SRC-01, PDF page 41 |

The screenshots also show INR as account currency and line-item display selected for these examples. The visible sort key is 001. The Machine, Cash Account, and Loan screenshots show the corresponding company-code currency / local-currency settings; verify individual account tabs before copying any additional values.

## 6. Accounts Payable and Accounts Receivable Examples

### Vendor examples in the implementation report

| Example | Organisational context | Details visible in source |
|---|---|---|
| Infineon Technologies | Domestic Vendor - HM11 | Vendor number appears as 2026202601; company code HM11; reconciliation account 1002; sort key 001; address shown as Harpy Street 512, Chennai 600018, India |
| Analog Devices Ltd | Foreign Vendor - HM12 | Named as the foreign-vendor example; the text does not provide a complete set of values |

Source: SRC-01, PDF pages 60-61. Do not publish supplier contact details beyond what is necessary for a portfolio example.

### Customer examples in the implementation report

The implementation report names **Mahindra Pvt Ltd** as the domestic customer example and **Berkshire Hathaway Ltd** as the foreign customer example (SRC-01, PDF pages 80-83).

A domestic customer reconciliation G/L example is visible as follows:

| Field | Value visible in source |
|---|---|
| G/L Account | 3 |
| Company Code | HM11 |
| Description | Sundry Debtors - Domestic |
| Account Group | AST ASSET |
| Account type | Balance Sheet |
| Reconciliation account type | D Customers |
| Currency | INR |
| Line-item display | Selected |
| Sort key | 001 |

Source: SRC-01, PDF page 72.

## 7. Controlling Snapshot

### Controlling Area

| Field | Value visible in source |
|---|---|
| Controlling Area | HM11 |
| Name | Controlling Area for HM11 |
| Validity shown | 2026 to 9999 |
| Company Code assignment option | 1 - Controlling area same as company code |
| Currency Type | 10 - Company Code Currency |
| Currency | INR |
| Chart of Accounts | HM11 |
| Fiscal Year Variant | HM (Jan-Dec) |
| Standard Hierarchy field | HM11-1 (as legible in the screenshot) |
| Active component | Cost Centers |
| Profit Center Accounting | Selected |
| Other indicator | All Currencies selected |

Source: SRC-01, PDF page 112.

### Profit Centre and Cost Centre examples

| Object | ID | Description | Other visible details | Source location |
|---|---|---|---|---|
| Profit Centre | HM11 | Production | Controlling Area HM11; responsible person label Production Manager; company code HM11 assigned; validity begins 01.01.2026; Profit Centre Group field shows HM11-1 | SRC-01, PDF page 114 |
| Profit Centre | HM12 | Marketing | Named as the Marketing Profit Centre example | SRC-01, PDF page 115 |
| Cost Centre | HM11-1 | Production | Controlling Area HM11; validity 01.04.2026 to 31.12.9999; category 1 (Production); hierarchy area HM11-1; Business Area HM21; currency INR; Profit Centre HM11 | SRC-01, PDF page 117 |
| Cost Centre | HM11-2 | Marketing | Controlling Area HM11; validity 01.04.2026 to 31.12.9999; category P (Marketing); hierarchy area HM11-1; Business Area HM21; currency INR; Profit Centre HM12 | SRC-01, PDF page 118 |

The Cost Centre screenshots show Functional Area HM11 with the description Manufacturing for both examples. Preserve this source value as shown, but validate the intended functional-area assignment before implementation.

## 8. Source-to-Portfolio Page Map

### SRC-01: Implementation report

| Source phase | PDF pages | Repository section |
|---|---:|---|
| Phase 1 - Enterprise Structure | 1-18 | [01-Enterprise-Structure](../01-Enterprise-Structure/README.md) |
| Phase 2 - Global Settings | 19-28 | [02-Global-Settings](../02-Global-Settings/README.md) |
| Phase 3 - General Ledger | 29-46 | [03-General-Ledger](../03-General-Ledger/README.md) |
| Phase 4 - Accounts Payable | 47-62 | [04-Accounts-Payable](../04-Accounts-Payable/README.md) |
| Phase 5 - Accounts Receivable | 63-83 | [05-Accounts-Receivable](../05-Accounts-Receivable/README.md) |
| Phase 6 - Asset Accounting | 84-110 | [06-Asset-Accounting](../06-Asset-Accounting/README.md) |
| Phase 7 - Controlling | 111-125 | [07-Controlling](../07-Controlling/README.md) |
| Phase 8 - Cutover Activities / Testing | 126-155 | [08-Cutover-and-Testing](../08-Cutover-and-Testing/README.md) |

### SRC-02: Business process report

| Process range | Area | Source PDF pages | Repository location |
|---|---|---:|---|
| 01-08 | General Ledger | 1-38 | [G/L business processes](../03-General-Ledger/business-processes/README.md) |
| 09-13 | Accounts Payable | 39-53 | [AP business processes](../04-Accounts-Payable/business-processes/README.md) |
| 14-19 | Accounts Receivable | 54-69 | [AR business processes](../05-Accounts-Receivable/business-processes/README.md) |
| 20-22 | Asset Accounting | 70-80 | [Asset business processes](../06-Asset-Accounting/business-processes/README.md) |
| 23-27 | Controlling | 81-92 | [CO business processes](../07-Controlling/business-processes/README.md) |

## 9. Source Differences and Items to Verify

The source reports are not perfectly consistent. These points are intentionally preserved rather than silently reconciled.

1. **Different vendor examples:** SRC-01 names Infineon Technologies (HM11) and Analog Devices Ltd (HM12). SRC-02 uses BE Solution Pvt Ltd and Sun IT Solutions for vendor master examples, and BE Solution Pvt Ltd for the rent invoice scenario.
2. **Different customer examples:** SRC-01 names Mahindra Pvt Ltd and Berkshire Hathaway Ltd. SRC-02 uses Unisoft Infotech Pvt Ltd and Zyple Software Solutions Pvt Ltd in its customer master and transaction examples.
3. **Cost Centre examples:** SRC-01 shows Production and Marketing cost centres. SRC-02 also refers to an HR Department cost-centre example.
4. **Vendor account-group assignment navigation:** SRC-01 section 4.3.1 is vendor-specific, but its navigation text refers to Customer Accounts / Customer Master Data. Verify the vendor-specific activity in the target SAP system.
5. **Segment procedure:** SRC-01 section 1.8 is titled Define Segment, but its steps refer to entering a Functional Area code and name. Verify the correct Segment object and field names.
6. **Direct G/L posting transaction:** SRC-02 Process 2 states FS00 for G/L posting, although SRC-01 Phase 8 names F-02 and FB50 for direct and indirect G/L posting. FS00 is identified elsewhere in SRC-02 for G/L master maintenance. Confirm the transaction used in the actual system.
7. **Customer line-item report:** SRC-02 Process 19 lists FS00 next to the G/L Line-item Report label. Other sections identify FBL3N for the G/L line-item report. Confirm the report code.
8. **Profit Centre prerequisite:** SRC-02 Process 27 lists Internal Order under Configuration Needed for Profit Centre creation. Confirm whether this is a project-specific dependency or a source-document error.
9. **Classic SAP GUI navigation:** The PDFs show classic SAP GUI procedures and transaction references. They do not establish that every screen or step was executed and verified in SAP S/4HANA Private Cloud 2025 or newer.

## 10. Evidence and Publication Rules

- Treat these values as **source-report examples**, not as automatically approved production configuration.
- Revalidate identifiers, account assignments, validity dates, and financial settings in the target SAP tenant before implementation.
- Replace or redact supplier, customer, employee, and financial details where publication would be inappropriate.
- Keep test cases marked **Not Executed** until a real system run and supporting evidence are attached.
- Do not claim FI/CO integration with SD, MM, or TM as completed; the supplied PDFs substantiate FI/CO only.
