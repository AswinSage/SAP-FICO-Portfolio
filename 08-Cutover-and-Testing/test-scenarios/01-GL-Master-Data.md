# Test Scenario 8.1 – G/L Master Data

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.1 G/L Master Data |
| Source procedure page | 126 |
| Source screenshot pages | 127–129 |
| Scenario category | Master data validation |
| Execution status | Executed – Completed (project completion confirmed by project owner) |

## Objective

Validate the creation of General Ledger master records with their Chart of Accounts and company-code segments, account classification, control data, currency, and field status.

## Source Procedure

1. Enter the G/L Account Number and Company Code.
2. Enter the Chart of Accounts where required.
3. Select Create.
4. Enter the Account Group and G/L Account Description.
5. Select the appropriate Account Type.
6. Maintain Control Data.
7. Enter the Currency and Field Status Group.
8. Verify mandatory fields and save.

The source demonstrates both **Balance Sheet Account Type** and **Profit & Loss Account Type** master records.

## Preconditions

- Company Code and Chart of Accounts exist.
- Account Group and Field Status Variant are configured.
- Retained Earnings Account assignment is available for P&L accounts.
- Required account number range and authorisations are active.

## Expected Results

- A G/L master record is created with the requested account number and description.
- Chart of Accounts data and company-code-specific data are available.
- Account Type and Account Group are consistent.
- Currency, Control Data, and Field Status Group are saved.
- The account can be displayed again and is available for subsequent posting, subject to posting controls.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Account identity | Account number and description are correct |
| Organisational assignment | Company Code and Chart of Accounts are correct |
| Classification | Account Group and Account Type are consistent |
| Control settings | Currency, Control Data and Field Status Group are maintained |
| P&L treatment | P&L account is associated with the relevant retained-earnings configuration |
| Display verification | Saved master record can be displayed |

## Source Screenshot Register

| PDF page | Screenshot subject |
|---:|---|
| 127 | G/L Master Data – Balance Sheet Account Type |
| 128 | G/L Master Data – Profit & Loss Account Type |
| 129 | Additional company-code / account-master screen states |

## Related Portfolio Scenarios

- [Create G/L Master Data](../../03-General-Ledger/business-processes/01-Create-GL-Master-Data.md)
- [G/L Direct Posting](../../03-General-Ledger/business-processes/02-General-Ledger-Direct-Posting.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.1, pages 126–129.
