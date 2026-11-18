# General Ledger (G/L)

## 1. Overview

General Ledger Accounting is the central accounting record for financial transactions. The uploaded SAP FICO implementation project identifies configuration activities for the Chart of Accounts, G/L Account Groups, Retained Earnings Account, and G/L Master Data.

The companion business-process document also describes operational G/L activities. These will be documented separately from configuration so that the project clearly distinguishes system setup from transaction execution.

## 2. Configuration Scope

| No. | Activity | Purpose |
|---:|---|---|
| 1 | Define Chart of Accounts | Establish the structured list of G/L accounts |
| 2 | Assign Company Code to Chart of Accounts | Link the company code to the account structure |
| 3 | Define Account Groups | Classify G/L accounts and control number ranges and screen layout |
| 4 | Define Retained Earnings Account | Maintain the account used for P&L balance carryforward |
| 5 | Create G/L Master Data | Maintain G/L account records at the relevant organizational levels |

## 3. Business Process Scope

The business-process document contains eight numbered G/L processes. The detailed process files will preserve the source process names and steps, with transaction codes and system evidence recorded only where supported.

## 4. Documentation Structure

| Folder | Contents |
|---|---|
| `configuration` | Chart of Accounts, assignments, account groups and retained earnings |
| `master-data` | G/L account master records |
| `business-processes` | G/L transaction procedures from the business-process document |
| `testing` | Test cases, expected results and actual evidence |
| `screenshots` | Redacted SAP system evidence |

## 5. Validation Approach

Configuration validation and transaction validation must be recorded separately. A saved configuration entry is not proof that a complete business transaction has been tested.

## 6. Source and Scope Note

Configuration scope is based on Phase 3, General Ledger, and the G/L master data activity in Phase 8 of the implementation project document. Operational G/L process scope is based on the G/L section of the companion business-process document.
