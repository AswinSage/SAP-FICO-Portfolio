# Process 10: Create Reconciliation G/L Account

## 1. Objective

Document creation of a reconciliation G/L account used to link vendor or customer sub-ledger balances with the General Ledger.

## 2. Business Purpose

The source explains that postings made to customer or vendor accounts automatically update the related reconciliation account in the General Ledger. Direct postings to reconciliation accounts are described as not allowed, preserving sub-ledger and G/L consistency.

## 3. Process Flow

- Preceding process: Nil
- Required process: Create Reconciliation G/L Account
- Succeeding process: Assign to Vendor and Customer Master Data

## 4. Prerequisites

**Configuration required**
- Chart of Accounts
- Account Group
- Retained Earnings Account
- Tolerance Group for G/L
- Field Status Variant

**Master data**
- G/L Master Data (`FS00`)

## 5. Procedure Outline

1. Open G/L master creation.
2. Select the relevant Chart of Accounts.
3. Enter the G/L account number.
4. Create the account and select the appropriate Account Group.
5. Enter the G/L account description.
6. Select the relevant balance sheet account type as described in the project.
7. Open Control Data.
8. Select the reconciliation account type appropriate to the sub-ledger.
9. Enter the company code and required Field Status Group.
10. Verify and save the account.

The source illustrates Sundry Debtors and Sundry Creditors reconciliation accounts.

## 6. Validation and Reporting

**Reports stated in source**
- G/L Line-item Report — `FBL3N`
- G/L Account Report — `FAGLB03`

- [ ] Reconciliation account is created.
- [ ] Correct sub-ledger reconciliation category is selected.
- [ ] Account is available for assignment in the relevant master data.
- [ ] G/L reports can display the account.

## 7. Evidence

**Source PDF screenshot pages:** 44-46 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`10-Create-Reconciliation-GL-Debtors.png` and `10-Create-Reconciliation-GL-Creditors.png`.

## 8. Implementation Notes

Keep vendor and customer reconciliation accounts distinct if the project uses separate accounts. Record the actual account category and assignment evidence.

## 9. Source Note

Business Processes document, Process 10, pages 43–46.