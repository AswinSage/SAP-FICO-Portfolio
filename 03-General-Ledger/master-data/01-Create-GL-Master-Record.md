# Create G/L Master Record

## 1. Objective

Document the creation of a General Ledger account master record for the project company code.

## 2. Business Purpose

A G/L Account Master contains the account information and control settings required to record financial transactions. The source project describes information maintained at the Chart of Accounts and Company Code levels, supporting correct account classification and financial reporting.

## 3. Master Data Activity

**Activity:** Create G/L Account Master

**SAP navigation:**

`SAP Easy Access → Accounting → Financial Accounting → General Ledger → Master Records → G/L Accounts → Individual Processing → Centrally`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the central G/L account master creation activity.
2. Enter the G/L Account Number.
3. Enter the Company Code.
4. Enter the Chart of Accounts, if required.
5. Select **Create**.
6. Enter the Account Group.
7. Enter the G/L Account Description.
8. Select the appropriate Account Type.
9. Maintain the Control Data.
10. Enter the Currency.
11. Enter the Field Status Group.
12. Verify all mandatory details.
13. Save the G/L master record.

## 5. Project Master Data Record

### Sample account values visible in the implementation report

| G/L account | Company Code | Description | Account Group | Account type | Source |
|---:|---|---|---|---|---|
| 1 | HM11 | Machine | AST ASSET | Balance Sheet | SRC-01, PDF page 35 |
| 2 | HM11 | Cash Account | AST ASSET | Balance Sheet | SRC-01, PDF page 37 |
| 1001 | HM11 | Loan / Loan Account | LIAB LIABILITY | Balance Sheet | SRC-01, PDF page 39 |
| 2001 | HM11 | Rent Account | EXP EXPENSES | P&L Statement | SRC-01, PDF page 41 |

The screenshots show INR account currency, line-item display selected, and sort key 001 for these sample records. Confirm each account's full company-code settings and Field Status Group in the live system; do not infer fields that are not visible.

## 6. Validation

- [ ] G/L account number is maintained.
- [ ] Company code and Chart of Accounts are correct.
- [ ] Account Group is valid for the Chart of Accounts.
- [ ] Description and account type are correct.
- [ ] Currency and Field Status Group are maintained.
- [ ] Master record is saved and can be displayed.

## 7. Evidence

Suggested screenshot: `05-Create-GL-Master-Record.png`

Use a non-confidential example account or redact sensitive financial details before publishing.

## 8. Implementation Notes

The source implementation document also includes a more detailed G/L master procedure under Phase 3, section 3.4. Capture any additional tabs or fields actually maintained in the project system. Do not assume that every optional field was configured.

## 9. Source Note

Based on Phase 3, section 3.4, G/L Master Data, and Phase 8, section 8.1, GL Master Data, in the uploaded SAP FICO implementation project document.
