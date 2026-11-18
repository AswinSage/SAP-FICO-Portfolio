# Cost Element Configuration Notes

## 1. Objective
Organize the cost element requirements documented across the implementation and business-process reports.

## 2. Source-Document Scope
The business-process document distinguishes:
- Primary Cost Element: originates outside CO and flows from FI, with a corresponding G/L account; source transaction `KA01`.
- Secondary Cost Element: used for internal allocations within CO; source transaction `KA06`.

The implementation project identifies Cost Elements as part of the Controlling scope. This file is an index and evidence register; record the exact configuration approach and cost element category used in the project system.

## 3. Required Relationships
| Element | Relationship to document |
|---|---|
| Primary Cost Element | Corresponding G/L account |
| Secondary Cost Element | Internal allocation between CO objects |
| Controlling Area | Organizational context |
| Cost Centre / Internal Order | Cost objects referenced by the source processes |

## 4. Evidence Register
| Item | Project value / evidence |
|---|---|
| Controlling Area | Record from SAP |
| Primary Cost Element | Record from SAP |
| Corresponding G/L Account | Record from SAP |
| Secondary Cost Element | Record from SAP |
| Cost Element Category | Record from SAP |
| Cost object assignment / posting | Record if performed |

## 5. Validation
- [ ] Primary cost element and corresponding G/L account are linked as intended.
- [ ] Secondary cost element category is checked.
- [ ] Controlling Area context is correct.
- [ ] Relevant cost objects exist.
- [ ] Posting and report evidence is available if tested.

## 6. Source Note
Business Processes document, Processes 23–24, pages 81–84; implementation project document, Phase 7.