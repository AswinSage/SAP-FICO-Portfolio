# Phase 8 – Cutover Activities and Testing

## 1. Phase Objective

Phase 8 validates that the SAP FICO master data and core accounting transactions established in the preceding implementation phases can support balanced postings, sub-ledger integration, document reversal, asset accounting, and transaction reporting.

The scope and sequence in this section follow **Phase 8: Cutover Activities – Testing** in the 155-page *SAP FICO Implementation Project Document*. The companion *SAP FICO Business Processes* PDF provides supporting business scenarios and process detail.

## 2. Source Scope

| Phase 8 activity | Source section | Source PDF pages | Test scenario |
|---|---|---:|---|
| G/L Master Data | 8.1 | [126](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=126)–[129](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=129) | Master record creation for Balance Sheet and Profit & Loss account types |
| G/L Posting | 8.2 | [130](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=130)–[132](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=132) | Direct posting (F-02) and indirect posting (FB50) |
| Reversal | 8.3 | [133](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=133)–[134](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=134) | Reverse an accounting document and retain the reversal reference |
| Vendor Invoice | 8.4 | [135](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=135)–[138](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=138) | Vendor liability and expense / asset posting |
| Vendor Payment | 8.5 | [139](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=139)–[141](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=141) | Payment and clearing of a vendor open item |
| Customer Invoice | 8.6 | [142](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=142)–[143](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=143) | Customer receivable and revenue posting |
| Customer Payment | 8.7 | [144](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=144)–[145](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=145) | Incoming payment and clearing of a customer open item |
| Asset Master Data | 8.8 | [146](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=146)–[152](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=152) | Single asset, group asset, and sub-asset master records |
| Asset Acquisition | 8.9 | [153](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=153)–[155](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=155) | External asset acquisition from a vendor using F-90 |

## 3. Test Workstreams and Dependencies

| Workstream | Prerequisite state | Downstream dependency |
|---|---|---|
| G/L master validation | Chart of Accounts, account groups, company-code settings, field status, retained earnings assignment | G/L postings, vendor/customer reconciliation accounts, asset account determination |
| G/L posting | Valid G/L masters, posting period, document controls, required cost objects | Reversal, line-item reporting, reconciliation |
| Document reversal | Original posted document, company code, fiscal year, reversal reason | Reversal audit trail and corrected balances |
| Vendor invoice | Vendor master, vendor reconciliation G/L, expense/asset G/L, posting period and tax settings where applicable | Vendor payment and AP/G/L reconciliation |
| Vendor payment | Posted vendor open item, bank/cash G/L, payment controls | Vendor clearing and bank/G/L reconciliation |
| Customer invoice | Customer master, customer reconciliation G/L, revenue G/L, posting period and tax settings where applicable | Customer payment and AR/G/L reconciliation |
| Customer payment | Posted customer open item, bank/cash G/L, incoming-payment controls | Customer clearing and bank/G/L reconciliation |
| Asset master | Asset class, chart of depreciation, depreciation area, account determination, number range, depreciation key | Asset acquisition, valuation and depreciation reporting |
| Asset acquisition | Valid asset master, vendor master, transaction type, asset and vendor account determination, posting period | Asset value update, vendor liability and G/L reconciliation |

## 4. End-to-End Test Sequence

The source sequence is organised into the following logical execution chain:

1. Confirm the G/L account structures and required G/L master records.
2. Validate direct and indirect G/L posting.
3. Reverse a posted G/L document and verify the linked reversal document.
4. Post a vendor invoice and confirm the vendor open item and corresponding G/L expense or asset entry.
5. Pay the vendor open item and verify the payment and clearing result.
6. Post a customer invoice and confirm the customer open item and revenue entry.
7. Receive customer payment and verify the payment and clearing result.
8. Create the required single, group, and sub-asset master records.
9. Post an external asset acquisition against a vendor and verify the asset and vendor accounting impact.

This sequence reflects the source scenarios. The PDFs do not define a complete production cutover calendar, downtime window, data-conversion load sequence, opening-balance migration, rollback plan, or formal go-live approval workflow.

## 5. Accounting and Control Assertions

| Transaction | Expected accounting effect | Core control assertion |
|---|---|---|
| Direct G/L expense posting | Debit expense / credit cash or bank, according to the source scenario | Total debits equal total credits; document is posted in the intended company code and period |
| G/L reversal | Reversal entries offset the original accounting document | Original document remains traceable; reversal document is linked and balances offset |
| Vendor invoice | Debit expense or asset (and input tax where applicable); credit vendor reconciliation account | Vendor open item and G/L impact agree; document balance is zero |
| Vendor payment | Debit vendor liability; credit bank/cash | Payment amount is assigned to the intended open item; clearing result is correct |
| Customer invoice | Debit customer reconciliation account; credit revenue (and output tax where applicable) | Customer open item and G/L impact agree; document balance is zero |
| Customer payment | Debit bank/cash; credit customer receivable | Receipt is assigned to the intended open item; clearing result is correct |
| Asset acquisition | Debit asset acquisition / APC account; credit vendor liability, subject to configured account determination and tax | Asset value and vendor liability are updated consistently; document balances |
| Asset master creation | No financial posting at master creation | Asset number, class, company code, depreciation terms and time-dependent assignments are valid |

The accounting effects above are the expected accounting logic for the source transaction types. Exact posting keys, tax treatment, account assignments, and ledger effects depend on the configured system and the specific transaction data.

## 6. Validation Layers

### 6.1 Master Data

- G/L account exists at Chart of Accounts and company-code levels.
- Vendor and customer masters contain the required company-code accounting data and reconciliation account.
- Asset master contains the intended asset class, organizational assignments, depreciation area, depreciation key, and useful life.
- Cost centre and profit centre assignments are valid where the transaction requires them.

### 6.2 Accounting Documents

- Company code, document date, posting date, currency, account assignments, and document header are consistent with the transaction.
- Debit and credit totals balance.
- The document is posted successfully and a document number is produced.
- Original and reversal documents remain traceable.

### 6.3 Sub-ledger and General Ledger Integration

- Vendor invoice and payment activity is reflected in vendor open-item and clearing status.
- Customer invoice and payment activity is reflected in customer open-item and clearing status.
- Reconciliation-account balances reflect the corresponding sub-ledger postings.
- Asset acquisition updates the asset value and the corresponding vendor / G/L accounting entries.

### 6.4 Reporting

The source documents identify the following report families for review:

| Area | Report / transaction reference in source |
|---|---|
| G/L line items | FBL3N |
| Vendor line items | FBL1N |
| Customer line items | FBL5N |
| Asset Explorer | AW01N |
| Asset List | AR01 |
| Asset balances | S_ALR_87011964 |
| Asset history sheet | S_ALR_87011990 |
| Cost element line items | KSB1 |
| Internal order actual line items | KOB1 |
| Profit centre line items | KE5Z |
| Profit centre actual line items | KE5Y |

Report availability and transaction-code compatibility depend on the SAP release and application configuration. The listed codes are source references, not a claim that each code is enabled in a current S/4HANA tenant.

## 7. Source Evidence Register

The implementation report contains screenshot pages for the Phase 8 activities:

| Activity | Screenshot pages | Source content |
|---|---:|---|
| G/L master | [127](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=127)–[129](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=129) | Balance Sheet and Profit & Loss account master screens |
| G/L posting | [131](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=131)–[132](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=132) | Direct posting screen labelled F-02 and indirect posting screen labelled FB50 |
| Reversal | 134 | Reversal entry and document display screens |
| Vendor invoice | [136](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=136)–[138](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=138) | Screens labelled Direct Posting – F-02 and Indirect Posting – FB60, with document display |
| Vendor payment | [140](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=140)–[141](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=141) | Outgoing payment and resulting posting screens |
| Customer invoice | 143 | Customer invoice entry screens |
| Customer payment | 145 | Incoming payment and resulting posting screens |
| Asset master | [147](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=147)–[152](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=152) | Single asset, group asset, and sub-asset screens |
| Asset acquisition | 154 | Screenshot page identified by the source as Asset Acquisition |

The text procedure pages are [126](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=126), [130](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=130), [133](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=133), [135](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=135), [139](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=139), [142](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=142), [144](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=144), [146](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=146), [153](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=153) respectively. Page 155 is the end of the source PDF.

## 8. Execution Status and Evidence Boundary

The SAP FICO project has been completed, and all nine Phase 8 scenarios are recorded as **Executed – Completed**. The implementation PDF provides the corresponding process descriptions and SAP screenshot references.

## 9. Source Limitations and Reconciliation Notes

1. Phase 8 labels G/L posting examples as F-02 and FB50 (pages 131–132). The companion Business Processes document describes G/L posting using FS00 in one place, despite using FS00 for G/L master maintenance. The Phase 8 references F-02 and FB50 are retained here as the Phase 8 source references; the discrepancy is recorded for verification.
2. The Vendor Invoice section (8.4) shows screenshots labelled F-02 and FB60 (pages 136–138). These labels are preserved as printed in the source. The PDF does not fully explain the difference between these paths.
3. The Sub-Asset subsection is identified on pages 151–152, but the source PDF contains limited extractable procedure text for these pages. The evidence page range is retained; detailed field-level steps are not inferred.
4. Asset Acquisition is described on page 153 and has a screenshot page at 154. The detailed screenshot content is not fully legible in the extracted copy; the transaction procedure is therefore based on the source text and the F-90 label.
5. The source does not provide a formal test result register, severity-based defect process, opening-balance migration procedure, cutover timetable, rollback design, or named approval sign-offs.

## 10. Phase 8 Conclusion

Phase 8 covers G/L master data, G/L postings, reversal, AP invoice and payment, AR invoice and payment, asset master creation, and external asset acquisition. The portfolio records these nine activities as executed and completed, based on the project owner's completion confirmation, with the corresponding procedure and screenshot references retained from the source report.
