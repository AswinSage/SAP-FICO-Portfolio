# Process 6: Unblock G/L at Company Code Level for Creation and Posting

## 1. Objective

Document removal of a G/L account block maintained at company code level.

## 2. Business Purpose

The source describes this activity as restoring the ability to use a previously blocked G/L account for accounting transactions within the relevant company code.

## 3. Process Flow

- Preceding process: Block G/L Master Data
- Required process: Unblock G/L Master Data
- Succeeding process: Posting

## 4. Prerequisites

- Configuration required: Nil, according to the source.
- Master data required: G/L Master Data.
- Transaction code stated in source: `FS00`.

## 5. Procedure Outline

1. Open the relevant G/L master record.
2. Select the company code segment.
3. Remove the block for creation and posting.
4. Save the updated master record.
5. Re-display the company code segment and verify the status.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] Company code-level block has been removed.
- [ ] The updated status is visible.
- [ ] A controlled posting test is documented if performed.

## 7. Evidence

Suggested evidence: `06-Unblock-GL-Company-Code-Level.png`.

## 8. Implementation Notes

Cross-reference Process 5. Capture the company code and G/L account details only if safe for public disclosure.

## 9. Source Note

Business Processes document, Process 6, pages 33–34.