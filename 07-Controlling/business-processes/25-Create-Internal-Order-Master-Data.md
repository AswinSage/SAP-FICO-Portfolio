# Process 25: Create Internal Order Master Data

## 1. Objective
Create an Internal Order to collect and monitor costs for a specific activity, project, event, or task.

## 2. Business Purpose
The source describes Internal Orders as cost collectors used to monitor budgets, actual costs, and settlements. Costs may later be settled to cost centers, assets, or profitability segments.

## 3. Process Flow
- Preceding: Nil
- Required: Internal Order
- Succeeding: Posting

## 4. Prerequisites
**Configuration:** Controlling Area, Order Type, Number Range for Internal Orders.

**Master data:** Internal Order Master (`KO01`).

## 5. Procedure Outline
1. Confirm the Controlling Area and order type.
2. Open Internal Order creation using `KO01`.
3. Enter the order type and required order details.
4. Maintain the description and organizational assignments.
5. Save and record the Internal Order number.
6. Display and verify the order.

Source example: Business Event.

## 6. Validation and Reporting
Report stated in source: Internal Order Actual Line Items (`KOB1`).
- [ ] Internal Order exists.
- [ ] Order type and Controlling Area are checked.
- [ ] Number range is verified.
- [ ] Order can be displayed.
- [ ] Actual line-item report can be reviewed after posting.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.86](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=86) · [PDF p.87](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=87). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).
Suggested: `25-Create-Internal-Order-Business-Event.png`.

## 8. Implementation Notes
Record the actual order type, number, and purpose. Document budgeting or settlement separately if performed.

## 9. Source Note
Business Processes document, Process 25, pages 85–87.