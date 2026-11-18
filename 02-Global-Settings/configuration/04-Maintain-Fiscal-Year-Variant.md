# Maintain Fiscal Year Variant

## 1. Objective

Maintain the Fiscal Year Variant that defines the accounting period structure used for financial transactions.

## 2. Business Purpose

The Fiscal Year Variant determines the number of posting periods and special periods available for accounting activities. It can follow the calendar year or another annual structure and is assigned to company codes to support period-based accounting and reporting.

## 3. Configuration Activity

**Configuration item:** Maintain Fiscal Year Variant

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Ledgers → Fiscal Year and Posting Periods → Maintain Fiscal Year Variant`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Maintain Fiscal Year Variant activity.
2. Select **New Entries**.
3. Enter the Fiscal Year Variant.
4. Enter the description.
5. Enter the number of posting periods.
6. Enter the number of special periods.
7. Define period start and end dates, if required by the project design.
8. Verify the mandatory details.
9. Save the variant.

## 5. Project Configuration Values

| Field | Value visible in SRC-01 |
|---|---|
| Fiscal Year Variant | HM |
| Description | Jan-Dec |
| Calendar year indicator | Selected |
| Number of posting periods | 12 |
| Number of special periods | 4 |

Source: implementation report, PDF page 23. The screenshot lists several fiscal-year variants; these values refer to the row labelled HM. Revalidate the selected variant and period definitions in the target SAP system.

## 6. Validation

- [ ] Fiscal Year Variant is created.
- [ ] Description is correct.
- [ ] Posting period count matches the project design.
- [ ] Special period count matches the project design.
- [ ] Period dates are checked, where maintained.
- [ ] Saved variant can be displayed.

## 7. Evidence

Suggested screenshot: `03-Maintain-Fiscal-Year-Variant.png`

## 8. Implementation Notes

Record the fiscal calendar decision and any non-calendar fiscal-year requirements. Do not fill period counts or dates without checking the actual project configuration.

## 9. Source Note

Based on Phase 2, section 2.2, Fiscal Year Variant, in the uploaded SAP FICO implementation project document.
