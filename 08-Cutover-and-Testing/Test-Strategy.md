# Test Strategy – Phase 8

## 1. Objective

The Phase 8 test strategy defines the validation model for the G/L, AP, AR and Asset Accounting scenarios documented in the implementation report. It establishes a consistent basis for comparing source procedures, accounting outcomes, sub-ledger updates, and report results.

## 2. Test Scope

| Test domain | Included validation |
|---|---|
| G/L master data | Balance Sheet and Profit & Loss account master creation |
| G/L posting | Direct and indirect posting, balancing and account assignment |
| Reversal | Reversal document generation and audit traceability |
| Accounts Payable | Vendor invoice recognition, outgoing payment and clearing |
| Accounts Receivable | Customer invoice recognition, incoming payment and clearing |
| Asset Accounting | Single, group and sub-asset master creation; external acquisition |
| Cross-module accounting | Vendor/customer sub-ledger integration with G/L and asset acquisition accounting |
| Reporting | G/L, vendor, customer, asset and relevant controlling report families |

## 3. Test Levels

| Test level | Test objective | Evidence class |
|---|---|---|
| Master-data validation | Confirm identity, organisational assignment and control data | Master-record display |
| Transaction validation | Confirm document header, line items, posting and document number | Posted accounting document |
| Sub-ledger integration | Confirm vendor/customer open items and reconciliation-account impact | Sub-ledger and G/L line-item output |
| Asset integration | Confirm asset master values and acquisition value updates | Asset master, Asset Explorer and accounting document |
| Reversal control | Confirm original/reversal relationship and offsetting accounting impact | Original and reversal document |
| Reporting validation | Confirm transaction records appear under the correct account and status | Relevant report output |

## 4. Execution Order and Dependency Model

The process dependency order is:

1. G/L master data and required reconciliation / expense / revenue / asset accounts.
2. G/L direct and indirect posting.
3. Document reversal.
4. Vendor master and reconciliation account, followed by vendor invoice.
5. Vendor payment and open-item clearing.
6. Customer master and reconciliation account, followed by customer invoice.
7. Customer payment and open-item clearing.
8. Asset master records, including single, group and sub-asset variants.
9. External asset acquisition using the source-stated F-90 path.

The sequence is a logical dependency model derived from the Phase 8 procedures and the related business-process documentation. It is not a production cutover calendar.

## 5. Core Assertions

- Master data is available under the intended organisational units.
- Accounting documents contain valid dates, company code, currency, accounts and line-item values.
- Debits and credits balance before posting.
- A successfully posted document receives a document number.
- Vendor and customer invoices create the expected open items.
- Vendor and customer payments are assigned to the intended open items.
- Reversal documents offset the original accounting impact without deleting the original record.
- Asset acquisition updates the asset value and the related vendor / G/L balances through configured account determination.
- The relevant line-item and asset reports reflect the underlying accounting records.

## 6. Evidence Classes

| Evidence class | Description | What it establishes |
|---|---|---|
| Source procedure | Textual procedure in the uploaded implementation PDF | Describes the intended process |
| Source screenshot | SAP screen image embedded in the uploaded implementation PDF | Shows a screen state represented in the source project report |
| Target-system execution | Current SAP tenant output with identifiable environment and execution reference | Establishes execution in the stated target environment |
| Reconciliation output | G/L/sub-ledger/asset report tied to the transaction | Supports financial and integration assertions |
| Review outcome | Dated review or approval record with accountable role | Establishes review/sign-off status |

Source screenshots are not automatically equivalent to target-system test evidence. The distinction is maintained in the Phase 8 register.

## 7. Test Status Definitions

| Status | Meaning |
|---|---|
| Executed – Completed | The project test scenario has been completed and is recorded as executed in the project register |
| Not Started | No execution record exists |
| In Progress | Execution has begun but the scenario is incomplete |
| Passed | Expected results are supported by current target-system evidence |
| Failed | Actual result differs from expected result |
| Blocked | A prerequisite, authorisation, configuration or system issue prevents completion |

For this portfolio, all nine Phase 8 scenarios are recorded as **Executed – Completed**, based on the project owner's confirmation that the implementation project has been completed.

## 8. Reporting References

| Functional area | Source report reference |
|---|---|
| General Ledger | FBL3N |
| Accounts Payable | FBL1N |
| Accounts Receivable | FBL5N |
| Asset Accounting | AW01N, AR01, S_ALR_87011964, S_ALR_87011990 |
| Controlling | KSB1, KOB1, KE5Z, KE5Y |

These are transaction/report references appearing in the project documents. Availability and compatibility depend on the target SAP release and configuration.

## 9. Source Limitations

- Phase 8 does not specify a complete defect severity model or defect resolution workflow.
- Phase 8 does not provide a formal test data catalogue or expected numeric balances for every scenario.
- The Sub-Asset section has limited extractable procedure text.
- The Vendor Invoice screenshots include captions F-02 and FB60; these source labels are preserved without treating them as a verified current-system mapping.
- The test strategy does not imply production go-live approval or successful execution in a target SAP tenant.

## 10. Source Note

Based on Phase 8, pages 126–155 of the *SAP FICO Implementation Project Document*, cross-referenced with the 27 process descriptions in *SAP FICO Business Processes*.
