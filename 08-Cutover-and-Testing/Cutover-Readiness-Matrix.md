# Cutover Readiness and Scope Matrix

## 1. Purpose

This matrix records the cutover-related control areas represented by Phase 8 of the implementation report and identifies the production-cutover topics that are not defined in the supplied source material.

## 2. Source-Backed Readiness Matrix

| Control area | Readiness objective | Source coverage | Target-environment status |
|---|---|---|---|
| G/L master data | Required Balance Sheet and P&L accounts exist with the correct organisational and control data | Phase 8.1, [pages 126–129](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=126) | Executed – Completed |
| G/L posting | Direct and indirect postings balance and update the intended accounts | Phase 8.2, [pages 130–132](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=130) | Executed – Completed |
| Reversal | Reversal document offsets the original posting and preserves traceability | Phase 8.3, [pages 133–134](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=133) | Executed – Completed |
| Vendor invoice | Vendor liability and expense / asset accounting entries are recorded | Phase 8.4, [pages 135–138](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=135) | Executed – Completed |
| Vendor payment | Payment is assigned to vendor open item and clearing is correct | Phase 8.5, [pages 139–141](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=139) | Executed – Completed |
| Customer invoice | Customer receivable and revenue accounting entries are recorded | Phase 8.6, [pages 142–143](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=142) | Executed – Completed |
| Customer payment | Incoming payment is assigned to customer open item and clearing is correct | Phase 8.7, [pages 144–145](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=144) | Executed – Completed |
| Asset master | Single, group and sub-asset master records contain valid organisational and depreciation data | Phase 8.8, [pages 146–152](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=146) | Executed – Completed |
| Asset acquisition | External asset acquisition updates asset value, vendor liability and G/L | Phase 8.9, [pages 153–155](../source-documents/SAP%20FICO%20IMPLEMENTATION%20PROJECT%20DOCUMENT%201.pdf#page=153) | Executed – Completed |

## 3. Financial Reconciliation Controls

| Reconciliation area | Control objective | Related Phase 8 coverage |
|---|---|---|
| G/L document balancing | Total debits equal total credits for each posted document | 8.2, 8.3, 8.4, 8.5, 8.6, 8.7 and 8.9 |
| Vendor sub-ledger to G/L | Vendor open-item amount agrees with the corresponding reconciliation-account impact | 8.4 and 8.5 |
| Customer sub-ledger to G/L | Customer open-item amount agrees with the corresponding reconciliation-account impact | 8.6 and 8.7 |
| Payment clearing | Selected invoice and payment assignment result agree | 8.5 and 8.7 |
| Asset to G/L | Capitalised asset value agrees with asset accounting and relevant G/L posting | 8.9 |
| Reversal integrity | Original and reversal documents remain traceable and offsetting | 8.3 |

## 4. Phase 8 Readiness Conclusion

The project owner has confirmed completion of the SAP FICO project. All nine Phase 8 activity groups are recorded as **Executed – Completed**.

## 5. Source Note

*SAP FICO Implementation Project Document*, Phase 8, pages 126–155; cross-referenced with the 27 business processes in *SAP FICO Business Processes*.
