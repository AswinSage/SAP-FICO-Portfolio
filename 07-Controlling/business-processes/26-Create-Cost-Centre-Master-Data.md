# Process 26: Create Cost Centre Master Data

## 1. Objective
Create a Cost Centre to collect and monitor costs incurred by a department or functional area.

## 2. Business Purpose
The source describes Cost Centres as department-level cost collectors supporting expense monitoring, cost allocation, budgeting, and management reporting. Examples include Production, HR, Finance, Marketing, and Administration.

## 3. Process Flow
- Preceding: Profit Centre
- Required: Create Cost Centre Master Data
- Succeeding: Linking to Cost Element or Posting

## 4. Prerequisites
**Configuration:** Controlling Area.

**Master data:** Cost Centre Master (`KS01`), Profit Centre (`KE51`).

## 5. Procedure Outline
1. Confirm the Controlling Area.
2. Confirm the relevant Profit Centre exists.
3. Open Cost Centre creation using `KS01`.
4. Enter the Cost Centre identifier and validity information.
5. Maintain name, description, and responsible organizational details.
6. Assign the relevant Profit Centre as required by the project.
7. Save and display the Cost Centre.

Source examples: Production Department, HR Department, Marketing Department.

## 6. Validation and Reporting
Report stated in source: Cost Centre Actual Line Items (`KSB1`).
- [ ] Cost Centre exists.
- [ ] Controlling Area and validity are correct.
- [ ] Profit Centre assignment is checked.
- [ ] Description is correct.
- [ ] Cost Centre can be used in relevant postings.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.89](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=89) · [PDF p.90](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=90). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).
Suggested: `26-Create-Cost-Centre-Production.png`, `26-Create-Cost-Centre-HR.png`, `26-Create-Cost-Centre-Marketing.png`.

## 8. Implementation Notes
Record the actual Cost Centre and Profit Centre assignments.

## 9. Source Note
Business Processes document, Process 26, pages 88–90.