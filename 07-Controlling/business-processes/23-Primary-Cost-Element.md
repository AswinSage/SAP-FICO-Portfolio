# Process 23: Primary Cost Element

## 1. Objective
Document a Primary Cost Element used to record costs originating outside Controlling and flowing from FI into CO.

## 2. Business Purpose
The source describes the primary cost element as a link between a G/L expense account and a cost object such as a cost center, internal order, or profit center. Examples include rent, salaries, electricity, and telephone charges. Each primary cost element must have a corresponding G/L account.

## 3. Process Flow
- Preceding: G/L Master Data
- Required: Primary Cost Element
- Succeeding: Posting

## 4. Prerequisites
**Configuration:** Controlling Area.

**Master data:** G/L Master (`FS00`), Primary Cost Element (`KA01`), Internal Order, Cost Center (`KS01`).

## 5. Procedure Outline
1. Confirm the Controlling Area.
2. Confirm the corresponding expense G/L account.
3. Create the primary cost element using the source-stated transaction.
4. Maintain the required cost element and controlling details.
5. Save and verify the cost element.
6. Confirm the relevant cost object is available for subsequent posting.

## 6. Validation and Reporting
Report stated in source: Cost Element Line Items (`KSB1`).
- [ ] Primary cost element exists.
- [ ] Corresponding G/L account is identified.
- [ ] Controlling Area is checked.
- [ ] Cost object is available.
- [ ] Report can be reviewed after posting.

## 7. Evidence

**Source PDF screenshot pages:** 82-83 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).
Suggested: `23-Primary-Cost-Element.png`.

## 8. Implementation Notes
Record the actual G/L and cost element relationship.

## 9. Source Note
Business Processes document, Process 23, pages 81–82.