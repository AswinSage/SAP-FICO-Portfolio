# Process 7: Reversal G/L – Rent Paid

## 1. Objective

Document reversal of an already-posted rent expense document.

## 2. Business Purpose

The source describes G/L reversal as the method for correcting an incorrectly posted transaction without deleting the original document. SAP creates a reversal document with opposite debit and credit entries to offset the original posting.

## 3. Process Flow

- Preceding process: Unblock G/L at Company Code Level for Creation and Posting
- Required process: Reversal G/L
- Succeeding process: G/L Line-item Report

## 4. Prerequisites

**Configuration required**
- Document Type
- Number Range
- Posting Period Variant
- Reversal Reason
- Posting Key
- Tolerance Group for G/L

**Master data**
- G/L Master (`FS00`)

## 5. Procedure Outline

1. Identify the original Rent Paid document to be reversed.
2. Verify the document number, company code, fiscal year, and posting details.
3. Open the reversal activity used in the project system.
4. Enter the original document reference and required reversal information.
5. Enter the reversal reason and posting date where required.
6. Execute the reversal and record the generated reversal document number.
7. Verify that the reversal offsets the original posting.

The source implementation report separately describes document reversal fields including document number, company code, fiscal year, reversal reason, and posting date.

## 6. Validation and Reporting

**Report stated in source:** G/L Line-item Report — `FBL3N`

- [ ] Original document remains available for audit trail.
- [ ] Reversal document is generated.
- [ ] Debit and credit effects offset the original posting.
- [ ] G/L line-item report reflects both documents.

## 7. Evidence

**Source PDF screenshot pages:** 36 in [SAP FICO BUSINESS PROCESSES (1).pdf](../../../../SAP%20FICO%20BUSINESS%20PROCESSES%20(1).pdf). See the [Screenshot Page Index](../../../00-Project-Overview/Screenshot-Page-Index.md) for the process-wise page map.

Suggested evidence: `07-Reversal-GL-Rent-Paid.png` and the related line-item report.

## 8. Implementation Notes

Record the original and reversal document references using redacted or sample data where necessary. Do not claim reversal completion without the reversal document evidence.

## 9. Source Note

Business Processes document, Process 7, pages 35–36; implementation project document, Phase 8 reversal procedure.