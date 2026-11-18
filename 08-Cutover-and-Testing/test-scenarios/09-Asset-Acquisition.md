# Test Scenario 8.9 – Asset Acquisition (F-90)

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.9 Asset Acquisition |
| Source procedure page | 153 |
| Source screenshot page | 154 |
| Transaction reference in source | F-90 |
| Scenario category | Asset acquisition and Accounts Payable integration |
| Execution in current target environment | Not independently verified |

## Objective

Validate an external asset acquisition from a vendor, including capitalisation of asset cost, vendor liability recognition, and the resulting Asset Accounting and General Ledger updates.

## Source Procedure

1. Enter Document Date and Posting Date.
2. Enter Company Code and Currency.
3. Enter Vendor Account.
4. Enter Asset Number.
5. Enter Transaction Type.
6. Enter Amount.
7. Enter Tax Code where applicable.
8. Verify Debit and Credit Entries.
9. Confirm that the document Balance is Zero.
10. Post the acquisition.

## Preconditions

- Asset master exists and is valid for the posting date.
- Vendor master exists with the relevant company-code accounting data.
- Asset class and account determination are configured.
- Asset transaction type is available.
- Posting period is open.
- Tax code is available where applicable.

## Expected Results

- Asset acquisition value is capitalised in the relevant asset record.
- Corresponding vendor liability is recorded.
- Relevant asset acquisition and reconciliation G/L accounts are updated through configured account determination.
- Tax entries are recorded where applicable.
- The accounting document balances to zero and a document number is generated.
- Asset value can be reviewed in the Asset Explorer and relevant asset reports.
- Vendor liability is available in vendor line-item reporting and can be settled through AP payment processing.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Document header | Dates, Company Code and Currency are correct |
| Vendor | Correct vendor is selected |
| Asset | Correct asset number is selected |
| Transaction Type | Valid acquisition transaction type is entered |
| Amount and tax | Acquisition amount and applicable tax are correct |
| Accounting document | Debit and credit values balance |
| Asset value | Capitalised value is reflected in the asset record |
| Vendor liability | Vendor open item is created |
| G/L integration | Asset and vendor reconciliation accounts are updated |

## Source Screenshot Register

- Page 153: Asset Acquisition explanation, navigation and procedure; transaction reference F-90.
- Page 154: Screenshot of the process.
- Page 155: End of the source PDF.

## Related Portfolio Scenarios

- [Create Single Asset Master](../../06-Asset-Accounting/business-processes/20-Create-Single-Asset-Master.md)
- [Asset Acquisition / External Acquisition](../../06-Asset-Accounting/business-processes/20-Create-Single-Asset-Master.md)
- [Vendor Payment](../../04-Accounts-Payable/business-processes/12-Vendor-Payment.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.9, pages 153–155. The process is explicitly labelled F-90 in the source report.
