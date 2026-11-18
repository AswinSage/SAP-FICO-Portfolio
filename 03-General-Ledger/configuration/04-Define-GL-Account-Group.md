# Define G/L Account Group

## 1. Objective

Define G/L Account Groups to classify G/L accounts and control account number ranges and master-record field behavior.

## 2. Business Purpose

An Account Group controls the creation and maintenance of G/L accounts. It determines the number range used for G/L account numbers and controls the screen layout of G/L master data fields, including required, optional, suppressed, or display-only settings.

## 3. Configuration Activity

**Configuration item:** Define Account Group

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → General Ledger Accounting → G/L Accounts → Master Data → Preparations → Define Account Group`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Define Account Group activity.
2. Select **New Entries**.
3. Enter the Chart of Accounts.
4. Enter the Account Group.
5. Enter the description.
6. Assign the From and To account number range.
7. Maintain the required Field Status settings.
8. Verify all mandatory details.
9. Save the Account Group.

## 5. Project Configuration Values

| Field | Project value |
|---|---|
| Chart of Accounts | To be recorded from SAP |
| Account Group | To be recorded from SAP |
| Description | To be recorded from SAP |
| From account number | To be recorded from SAP |
| To account number | To be recorded from SAP |
| Field Status settings | Record actual settings |

## 6. Validation

- [ ] Chart of Accounts is selected correctly.
- [ ] Account Group identifier and description are maintained.
- [ ] Account number range is recorded and checked.
- [ ] Field Status settings match the project requirement.
- [ ] Saved Account Group can be displayed.

## 7. Evidence

Suggested screenshot: `03-Define-GL-Account-Group.png`

## 8. Implementation Notes

Record the account classification logic and number range decisions actually used. Do not create or publish arbitrary ranges as project facts.

## 9. Source Note

Based on Phase 3, section 3.2, Account Group, in the uploaded SAP FICO implementation project document.
