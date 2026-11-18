# Define Chart of Accounts

## 1. Objective

Define the Chart of Accounts used as the structured list of G/L accounts for financial recording and reporting.

## 2. Business Purpose

A Chart of Accounts provides a common framework of G/L accounts used by one or more company codes. It supports consistent classification and reporting of financial transactions.

## 3. Configuration Activity

**Configuration item:** Edit Chart of Accounts List

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → General Ledger Accounting → G/L Accounts → Master Data → Preparations → Edit Chart of Accounts List`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Edit Chart of Accounts List activity.
2. Select **New Entries**.
3. Enter the four-character Chart of Accounts identifier.
4. Enter the description.
5. Enter the maintenance language.
6. Select the length of the G/L account number.
7. Select Controlling Integration, if required by the project.
8. Verify all mandatory details.
9. Save the Chart of Accounts.

## 5. Project Configuration Values

| Field | Project value |
|---|---|
| Chart of Accounts | To be recorded from SAP |
| Description | To be recorded from SAP |
| Maintenance language | To be recorded from SAP |
| G/L account number length | To be recorded from SAP |
| Controlling integration | Record actual selection |

## 6. Validation

- [ ] Chart of Accounts identifier is maintained.
- [ ] Description and maintenance language are correct.
- [ ] G/L account number length matches the project design.
- [ ] Controlling integration selection is checked, if applicable.
- [ ] Saved Chart of Accounts can be displayed.

## 7. Evidence

Suggested screenshot: `01-Define-Chart-of-Accounts.png`

## 8. Implementation Notes

Record the actual identifier and settings used in the project system. Do not use sample values as if they were project values.

## 9. Source Note

Based on Phase 3, section 3.1, Chart of Accounts, in the uploaded SAP FICO implementation project document.
