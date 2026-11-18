# Enterprise Structure

## 1. Overview
Enterprise Structure defines the organizational framework used by the SAP FICO project. It establishes the company, company code, and related organizational units and assignments that provide the foundation for financial accounting and reporting.

## 2. Configuration Scope
The source implementation report identifies the following activities:

1. Define Company
2. Define Company Code
3. Assign Company Code to Company
4. Define Credit Control Area
5. Assign Company Code to Credit Control Area
6. Define Business Area
7. Assign Business Area to Consolidation Business Area
8. Define Functional Area
9. Define Consolidation Business Area
10. Define Financial Management Area
11. Assign Company Code to Financial Management Area
12. Define Segment

## 3. Configuration Documentation
| File | Activity |
|---|---|
| [Configuration Overview](configuration/01-Enterprise-Structure-Configuration-Overview.md) | Full activity register and validation checklist |
| [Define Company](configuration/02-Define-Company.md) | Company definition |
| [Define Company Code](configuration/03-Define-Company-Code.md) | Company Code definition |
| [Assign Company Code to Company](configuration/04-Assign-Company-Code-to-Company.md) | Company / company code relationship |
| [Define Credit Control Area](configuration/05-Define-Credit-Control-Area.md) | Credit management organizational unit |
| [Assign Company Code to Credit Control Area](configuration/06-Assign-Company-Code-to-Credit-Control-Area.md) | Credit control assignment |
| [Define Business Area](configuration/07-Define-Business-Area.md) | Business Area definition |
| [Assign Business Area to Consolidation Business Area](configuration/08-Assign-Business-Area-to-Consolidation-Business-Area.md) | Consolidation assignment |
| [Define Functional Area](configuration/09-Define-Functional-Area.md) | Functional reporting unit |
| [Define Consolidation Business Area](configuration/10-Define-Consolidation-Business-Area.md) | Consolidation unit definition |
| [Define Financial Management Area](configuration/11-Define-Financial-Management-Area.md) | Funds management organizational unit |
| [Assign Company Code to Financial Management Area](configuration/12-Assign-Company-Code-to-Financial-Management-Area.md) | Financial Management assignment |
| [Define Segment](configuration/13-Define-Segment.md) | Segment configuration procedure as written in source |

## 4. Supporting Material
- `notes/`: Conceptual notes
- `diagrams/`: Organizational diagrams
- `business-scenarios/`: Business examples
- `screenshots/`: Redacted SAP evidence

## 5. Validation
- [ ] Organizational unit definitions are saved.
- [ ] Company code assignments are verified.
- [ ] Relationships match the project design.
- [ ] Screenshots or configuration evidence are attached.

## 6. Source-Document Verification
The source document's Segment procedure refers to Functional Area fields. This is flagged in the corresponding configuration file and must be checked against the actual SAP system.

## 7. Source Note
Implementation project document, Phase 1, sections 1.1–1.8.

## Source PDF References

- **SRC-01 – Implementation Project Document:** Phase 1, Enterprise Structure, pages 1–18.
- Central index: [Source Documents](../source-documents/README.md).
