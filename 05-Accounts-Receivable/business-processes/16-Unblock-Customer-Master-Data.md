# Process 16: Unblock Customer Master Data

## 1. Objective

Document removal of a restriction from a previously blocked customer master record.

## 2. Business Purpose

The source describes unblocking as the action taken when a customer becomes eligible for business transactions again. It notes that unblocking may be maintained at company code, sales area, or central level depending on business requirements.

## 3. Process Flow

- Preceding process: Block Customer Master Data
- Required process: Unblock Customer Master Data
- Succeeding process: Customer Invoice

## 4. Prerequisites

- Configuration required: None.
- Master data required: Customer Master Data (`XD01`).

## 5. Procedure Outline

1. Identify the customer previously blocked in Process 15.
2. Open the relevant customer master maintenance activity.
3. Locate the block at the organizational level used in the project.
4. Remove the relevant block.
5. Save the change.
6. Display the customer record and verify the updated status.

## 6. Validation and Reporting

**Reports stated in source**
- Customer Line-item Report — `FBL5N`
- G/L Line-item Report — `FBL3N`

- [ ] Correct customer is selected.
- [ ] Relevant block is removed.
- [ ] Updated status can be displayed.
- [ ] A controlled subsequent transaction test is documented if performed.

## 7. Evidence

**Source PDF screenshot pages:** [PDF p.61](https://github.com/AswinSage/SAP-FICO-Portfolio/blob/main/source-documents/SAP%20FICO%20BUSINESS%20PROCESSES.pdf#page=61). See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`16-Unblock-Customer-Master.png`.

## 8. Implementation Notes

Cross-reference Process 15 and record whether the block was removed at company code, sales area, or central level.

## 9. Source Note

Business Processes document, Process 16, pages 60–61.