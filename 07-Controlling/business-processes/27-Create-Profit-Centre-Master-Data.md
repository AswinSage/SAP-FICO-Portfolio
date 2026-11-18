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

Source example in SRC-02: **Custom Product**.

### Additional project examples in the implementation report (SRC-01)

The implementation report shows two Profit Centre master examples:

| Profit Centre | Description | Controlling Area | Company Code assignment | Other source details |
|---|---|---|---|---|
| HM11 | Production | HM11 | HM11 assigned | Validity begins 01.01.2026; Profit Centre Group field shows HM11-1; responsible-person label shown as Production Manager |
| HM12 | Marketing | Not fully visible in the example caption | Not fully visible | Named as the Marketing Profit Centre example |

Sources: SRC-01, PDF pages 114-115. These examples are from the implementation report and are distinct from the Custom Product scenario in the 92-page business-process PDF. Confirm all assignments and validity dates in the target SAP system.

## 6. Validation and Reporting
Reports stated in source: Profit Centre Line Items (`KE5Z`); Profit Centre Actual Line Items (`KE5Y`).
- [ ] Profit Centre exists.
- [ ] Controlling Area and Standard Hierarchy context are checked.
- [ ] Description and validity are correct.
- [ ] Profit Centre is available for Cost Centre assignment.
- [ ] Reports can be executed after postings.

## 7. Evidence

**Source PDF screenshot pages:** 91-92 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).
Suggested: `27-Create-Profit-Centre-Custom-Product.png`.

## 8. Implementation Notes
The source lists Internal Order under Configuration Needed. Preserve this source reference, but verify the intended dependency against the actual project design before treating it as a mandatory prerequisite.

## 9. Source Note
Business Processes document, Process 27, pages 90–92.