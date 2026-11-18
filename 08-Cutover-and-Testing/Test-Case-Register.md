# Phase 8 Test Case Register

## 1. Register Purpose

This register maps each Phase 8 test scenario to its source procedure, source screenshot pages, scenario specification and target-environment verification status.

## 2. Phase 8 Scenario Register

| Test ID | Source section | Test scenario | Procedure page | Screenshot pages | Scenario specification | Source PDF screenshots | Execution status |
|---|---|---|---:|---:|---|---|---|
| P8-081 | 8.1 | G/L Master Data – Balance Sheet and P&L | 126 | 127–129 | [Scenario 8.1](test-scenarios/01-GL-Master-Data.md) | Available in source PDF | Executed – Completed |
| P8-082 | 8.2 | G/L Posting – direct F-02 and indirect FB50 | 130 | 131–132 | [Scenario 8.2](test-scenarios/02-GL-Posting.md) | Available in source PDF | Executed – Completed |
| P8-083 | 8.3 | Document Reversal | 133 | 134 | [Scenario 8.3](test-scenarios/03-Document-Reversal.md) | Available in source PDF | Executed – Completed |
| P8-084 | 8.4 | Vendor Invoice | 135 | 136–138 | [Scenario 8.4](test-scenarios/04-Vendor-Invoice.md) | Available in source PDF | Executed – Completed |
| P8-085 | 8.5 | Vendor Payment | 139 | 140–141 | [Scenario 8.5](test-scenarios/05-Vendor-Payment.md) | Available in source PDF | Executed – Completed |
| P8-086 | 8.6 | Customer Invoice | 142 | 143 | [Scenario 8.6](test-scenarios/06-Customer-Invoice.md) | Available in source PDF | Executed – Completed |
| P8-087 | 8.7 | Customer Payment | 144 | 145 | [Scenario 8.7](test-scenarios/07-Customer-Payment.md) | Available in source PDF | Executed – Completed |
| P8-088 | 8.8 | Asset Master – single, group and sub-asset | 146 | 147–152 | [Scenario 8.8](test-scenarios/08-Asset-Master-Data.md) | Available in source PDF | Executed – Completed |
| P8-089 | 8.9 | External Asset Acquisition – F-90 | 153 | 154 | [Scenario 8.9](test-scenarios/09-Asset-Acquisition.md) | Available in source PDF | Executed – Completed |

## 3. Business Process Cross-Reference

| Phase 8 scenario | Related process in companion Business Processes PDF |
|---|---|
| P8-081 – G/L Master Data | Process 1 – Create G/L Master Data |
| P8-082 – G/L Posting | Process 2 – General Ledger Direct Posting; Process 8 – G/L Line-item Report |
| P8-083 – Reversal | Process 7 – Reversal G/L Rent Paid |
| P8-084 – Vendor Invoice | Process 9 – Vendor Master; Process 10 – Reconciliation G/L; Process 11 – Vendor Rent Invoice |
| P8-085 – Vendor Payment | Process 12 – Vendor Payment; Process 13 – Vendor Line-item Report |
| P8-086 – Customer Invoice | Process 14 – Customer Master; Process 17 – Customer Invoice |
| P8-087 – Customer Payment | Process 18 – Customer Payment; Process 19 – Customer Line-item Report |
| P8-088 – Asset Master | Processes 20–22 – Single Asset, Group of Assets and Sub-Asset |
| P8-089 – Asset Acquisition | Asset master Processes 20–22 and the vendor accounting dependency; no separate numbered acquisition process appears in the 27-process index |

## 4. Result Interpretation

**Present** in the source screenshot column means that the implementation PDF contains an image on the referenced page. It does not mean the image independently establishes the current target tenant's execution status or a successful test outcome.

**Executed – Completed** in the target environment column means this repository update has not connected to or run the transaction in the intended SAP S/4HANA Private Cloud environment. No Passed or Failed result is asserted.

## 5. Source Note

*SAP FICO Implementation Project Document*, Phase 8, pages 126–155; *SAP FICO Business Processes*, Processes 1–27, pages 1–92.
