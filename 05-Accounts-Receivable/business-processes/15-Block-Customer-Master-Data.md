# Process 15: Block Customer Master Data

## 1. Objective

Document blocking of a customer master record at the level described in the source project.

## 2. Business Purpose

The source identifies customer blocking as a control that may be used for credit issues, business closure, duplicate records, or temporary restrictions. It states that the block can be maintained at company code level and that the effect depends on the block level applied.

## 3. Process Flow

- Preceding process: Create Customer Master Data
- Required process: Block Customer Master Data
- Succeeding process: Unblock Customer Master Data

## 4. Prerequisites

- Configuration required: Nil, according to the source.
- Master data / transaction stated in source: Customer Block Screen (`FD05`).

## 5. Procedure Outline

1. Identify the customer master record to be blocked.
2. Open the customer blocking activity stated in the source.
3. Select the relevant customer and organizational scope.
4. Apply the block at the level used in the project.
5. Save the change.
6. Display the customer record and verify the block status.

## 6. Validation and Reporting

**Reports stated in source**
- Customer Line-item Report — `FBL5N`
- G/L Line-item Report — `FBL3N`

- [ ] Correct customer is selected.
- [ ] Block level is recorded.
- [ ] Block status is visible in the master record.
- [ ] Any posting restriction test is documented if performed.

## 7. Evidence

Suggested evidence: `15-Block-Customer-Master.png`.

## 8. Implementation Notes

Record the exact block scope used. Do not claim that all sales and accounting activities are blocked unless the actual configuration and test establish that result.

## 9. Source Note

Business Processes document, Process 15, pages 58–59.