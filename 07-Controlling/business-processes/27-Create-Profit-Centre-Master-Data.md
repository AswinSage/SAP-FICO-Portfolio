# Process 27: Create Profit Centre Master Data

## 1. Objective
Create a Profit Centre to analyze profitability for a business area, product line, branch, or department.

## 2. Business Purpose
The source describes Profit Centres as units for evaluating revenues, costs, and profit independently. It states that each Profit Centre is assigned to a Controlling Area and Standard Hierarchy.

## 3. Process Flow
- Preceding: Nil
- Required: Create Profit Centre Master Data
- Succeeding: Assign to Cost Centre

## 4. Prerequisites
**Configuration listed in source:** Internal Order.

**Master data:** Profit Centre Master (`KE51`).

## 5. Procedure Outline
1. Confirm the Controlling Area and Standard Hierarchy context.
2. Open Profit Centre creation using `KE51`.
3. Enter the Profit Centre identifier and required organizational data.
4. Maintain description and validity information.
5. Save and display the Profit Centre.
6. Record its assignment to the relevant Cost Centre when that subsequent activity is performed.

Source example: Custom Product.

## 6. Validation and Reporting
Reports stated in source: Profit Centre Line Items (`KE5Z`); Profit Centre Actual Line Items (`KE5Y`).
- [ ] Profit Centre exists.
- [ ] Controlling Area and Standard Hierarchy context are checked.
- [ ] Description and validity are correct.
- [ ] Profit Centre is available for Cost Centre assignment.
- [ ] Reports can be executed after postings.

## 7. Evidence
Suggested: `27-Create-Profit-Centre-Custom-Product.png`.

## 8. Implementation Notes
The source lists Internal Order under Configuration Needed. Preserve this source reference, but verify the intended dependency against the actual project design before treating it as a mandatory prerequisite.

## 9. Source Note
Business Processes document, Process 27, pages 90–92.