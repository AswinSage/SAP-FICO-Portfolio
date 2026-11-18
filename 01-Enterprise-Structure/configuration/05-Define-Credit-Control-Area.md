# Define Credit Control Area

## 1. Objective
Define the Credit Control Area used to manage and monitor customer credit limits.

## 2. Business Purpose
The source describes this organizational unit as supporting centralized monitoring of customer credit exposure, utilization, and payment behavior across assigned company codes.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Enterprise Structure → Definition → Financial Accounting → Define Credit Control Area`

## 4. Procedure
1. Select New Entries.
2. Enter the four-digit Credit Control Area.
3. Enter the Description.
4. Select the Currency.
5. Enter Update and Fiscal Year Variant settings.
6. Enter the Credit Limit.
7. Maintain Risk Category settings, if applicable.
8. Verify mandatory fields and save.

## 5. Project Values
| Field | Value visible in SRC-01 |
|---|---|
| Credit Control Area | HM11 |
| Description | Credit Control Area - HM11 |
| Currency | INR |
| Fiscal Year Variant field | H1 |
| Credit Limit | 1,500,000,000 |
| Update setting / Risk Category | Not transcribed; value is not sufficiently clear in the screenshot |

Source: implementation report, PDF page 7. Revalidate all entries in the target SAP system before reuse.

## 6. Validation
- [ ] Credit Control Area exists.
- [ ] Currency and fiscal year settings are checked.
- [ ] Credit limit and risk settings are reviewed.
- [ ] Saved configuration can be displayed.

## 7. Evidence
Suggested: `05-Define-Credit-Control-Area.png`.

## 8. Source Note
Implementation project document, Phase 1, section 1.3.