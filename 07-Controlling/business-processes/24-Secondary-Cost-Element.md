# Process 24: Secondary Cost Element

## 1. Objective
Document creation of a Secondary Cost Element for internal cost allocation within CO.

## 2. Business Purpose
The source describes secondary cost elements as being used for internal allocations such as assessments, distributions, activity allocations, and overhead calculations. It states that they do not have a corresponding G/L account in FI.

## 3. Process Flow
- Preceding: Nil
- Required: Secondary Cost Element
- Succeeding: Linking with Internal Order

## 4. Prerequisites
**Configuration:** Controlling Area.

**Master data:** Secondary Cost Element (`KA06`), Internal Order (`KO01`), Cost Center (`KS01`).

## 5. Procedure Outline
1. Confirm the Controlling Area.
2. Open Secondary Cost Element creation using the source-stated transaction.
3. Enter the required cost element details and category.
4. Save and verify the cost element.
5. Confirm the relevant internal order and cost center are available.

## 6. Validation and Reporting
Report stated in source: Cost Element Line Items (`KSB1`).
- [ ] Secondary cost element exists.
- [ ] Controlling Area and category are checked.
- [ ] Relevant cost objects are available.
- [ ] Allocation/posting evidence is recorded if performed.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.84](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=84) · [PDF p.85](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=85). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).
Suggested: `24-Secondary-Cost-Element.png`.

## 8. Implementation Notes
Record the actual category and settings from the SAP system.

## 9. Source Note
Business Processes document, Process 24, pages 83–84.