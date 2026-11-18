# Internal Order Configuration Notes

## 1. Objective
Document the configuration prerequisites for Internal Order master data identified in the source project.

## 2. Source-Document Scope
The Business Processes document identifies the following prerequisites:
- Controlling Area
- Order Type
- Number Range for Internal Orders

It identifies `KO01` for Internal Order master creation. The implementation project also includes Internal Orders in the Controlling scope.

## 3. Configuration Evidence Register
| Item | Project value |
|---|---|
| Controlling Area | Record from SAP |
| Order Type | Record from SAP |
| Number Range | Record from SAP |
| Number range interval | Record from SAP |
| Internal Order master | Record from SAP |

## 4. Validation
- [ ] Controlling Area is available.
- [ ] Required Order Type is maintained.
- [ ] Number range is maintained and assigned as applicable.
- [ ] Internal Order can be created and displayed.
- [ ] Actual line-item reporting can be reviewed after posting.

## 5. Source Note
Business Processes document, Process 25, pages 85–87.