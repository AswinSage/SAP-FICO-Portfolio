# Define Retained Earnings Account

## 1. Objective

Document the Retained Earnings Account configuration used for carrying forward profit and loss account balances.

## 2. Business Purpose

The Retained Earnings Account is used to carry forward the balances of profit and loss accounts to the next fiscal year. The source project describes the account as supporting the transfer of the previous year's profit or loss to the balance sheet during year-end closing.

## 3. Configuration Activity

**Configuration item:** Define Retained Earnings Account

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → General Ledger Accounting → G/L Accounts → Master Data → Preparations → Define Retained Earnings Account`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Define Retained Earnings Account activity.
2. Enter the Chart of Accounts.
3. Select **New Entries**, if required.
4. Enter the P&L Statement Account Type.
5. Complete the remaining required fields as presented by the project system.
6. Verify the configuration.
7. Save the entry.

## 5. Project Configuration Values

| Field | Value visible in SRC-01 |
|---|---|
| Chart of Accounts | HM11 |
| P&L Statement Account Type | BIL |
| Retained Earnings G/L Account | 1000 |

Source: implementation report, PDF page 33. These are source-report values; validate the account assignment in the target SAP system.

## 6. Validation

- [ ] Correct Chart of Accounts is selected.
- [ ] P&L Statement Account Type is maintained.
- [ ] Retained earnings account assignment is checked in the system.
- [ ] Saved configuration can be displayed.

## 7. Evidence

Suggested screenshot: `04-Define-Retained-Earnings-Account.png`


## 8. Source Note

Based on Phase 3, section 3.3, Retained Earnings Account, in the uploaded SAP FICO implementation project document.
