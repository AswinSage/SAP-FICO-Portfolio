# Reports and Validation

## 1. Overview
This section consolidates the reports referenced across the SAP FICO implementation and business-process documents. It provides a central place to document selection criteria, business purpose, validation checks, and evidence.

## 2. Report Index
| Area | Report / transaction | Purpose in source documents |
|---|---|---|
| G/L | `FBL3N` | G/L line-item report |
| G/L | `FAGLB03` | G/L account balance/report reference |
| AP | `FBL1N` | Vendor line-item report |
| AR | `FBL5N` | Customer line-item report |
| Asset Accounting | `AW01N` | Asset Explorer |
| Asset Accounting | `AR01` | Asset List |
| Asset Accounting | `S_ALR_87011964` | Asset Balances |
| Asset Accounting | `S_ALR_87011990` | Asset History Sheet |
| CO | `KSB1` | Cost Centre / cost element line items as referenced |
| CO | `KOB1` | Internal Order actual line items |
| CO | `KE5Z` | Profit Centre line items |
| CO | `KE5Y` | Profit Centre actual line items |

## 3. Validation Standard
For each report, record the transaction or app actually used, selection parameters, company code or controlling context, date range, expected source documents, actual result, and evidence.

## 4. Source-Document Inconsistencies
The Business Processes document labels the G/L Line-item Report as `FBL3N` in multiple places but includes `FS00` in the Process 19 report list next to a G/L Line-item Report label. Verify this against the project system before publishing the Process 19 report code as final.

## 5. Source Note
Compiled from the report references in the SAP FICO Business Processes document, Processes 1–27, and the implementation project document.

## Source PDF References

- **[SRC-01 – Implementation Project Document](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf):** Phase-specific configuration and Phase 8 testing references, pages 1–155.
- **[SRC-02 – Business Processes](../source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf):** Process-specific validation and report references, pages 1–92.
- Central index: [Source Documents](../source-documents/README.md).
