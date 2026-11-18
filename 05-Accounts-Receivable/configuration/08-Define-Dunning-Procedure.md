# Define Dunning Procedure

## 1. Objective
Define the dunning procedure used to structure follow-up activities for overdue open items.

## 2. Business Purpose
The source describes a Dunning Procedure as defining dunning levels, minimum days in arrears, dunning intervals, grace periods, and charges where applicable. It supports systematic follow-up of overdue receivables or payables.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Accounts Receivable and Accounts Payable → Business Transactions → Dunning → Dunning Procedure → Define Dunning Procedures`

## 4. Procedure
1. Select New Entries.
2. Enter the four-character Dunning Procedure.
3. Enter the Description.
4. Enter the Dunning Interval in Days.
5. Enter the Number of Dunning Levels.
6. Maintain Minimum Days in Arrears for each level.
7. Maintain Dunning Charges, if required.
8. Maintain Grace Days, if required.
9. Select the relevant Dunning Level.
10. Maintain required Dunning Form/Texts, if applicable.
11. Verify mandatory details and save.

## 5. Project Values
| Field | Project value |
|---|---|
| Dunning Procedure | Record from SAP |
| Description | Record from SAP |
| Dunning Interval | Record from SAP |
| Number of Dunning Levels | Record from SAP |
| Minimum Days in Arrears | Record per level |
| Dunning Charges | Record if used |
| Grace Days | Record if used |
| Dunning Form / Text | Record if used |

## 6. Validation
- [ ] Dunning procedure exists.
- [ ] Interval and number of levels are correct.
- [ ] Minimum days in arrears are maintained.
- [ ] Charges and grace days are checked where applicable.
- [ ] Dunning procedure is available for assignment and processing.

## 7. Evidence
Suggested: `07-Define-Dunning-Procedure.png`.

## 8. Implementation Notes
Record the actual dunning levels and parameters. Do not imply that a dunning run was executed unless separate run evidence exists.

## 9. Source Note
Implementation project document, Phase 5, section 5.6.