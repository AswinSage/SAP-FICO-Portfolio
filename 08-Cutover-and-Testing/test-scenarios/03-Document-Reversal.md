# Test Scenario 8.3 – Document Reversal

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.3 Reversal |
| Source procedure pages | 133–134 |
| Source screenshot page | 134 |
| Scenario category | Accounting control validation |
| Execution status | Executed – Completed |

## Objective

Validate cancellation of an incorrectly posted accounting document through a corresponding reversal document while preserving the original document for audit traceability.

## Source Procedure

1. Enter the original Document Number.
2. Enter the Company Code and Fiscal Year.
3. Enter the Reversal Reason.
4. Enter the Posting Date where required.
5. Verify the document details.
6. Save the reversal.
7. Confirm the generated Reversal Document Number.

## Preconditions

- The original accounting document exists and is eligible for reversal.
- The reversal posting period is open.
- A valid reversal reason is configured.
- The original document's company code and fiscal year are known.

## Expected Results

- A reversal document is generated.
- The reversal document references the original transaction through the document relationship.
- The original document remains available for display and audit.
- The reversal entries offset the accounting impact of the original document, subject to reversal scope and period rules.
- The generated reversal document number is recorded.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Original document | Correct original number, company code and fiscal year |
| Reversal controls | Valid reversal reason and posting date |
| Reversal result | Reversal document posted successfully |
| Audit trail | Original and reversal documents are both displayable |
| Financial effect | Reversal offsets the original values in the relevant accounts |
| Period control | Reversal posting is in a valid open period |

## Source Screenshot Register

Page 134 contains the reversal entry screen and resulting reversal-document display.

## Related Portfolio Scenarios

- [G/L Direct Posting](../../03-General-Ledger/business-processes/02-General-Ledger-Direct-Posting.md)
- [Reversal of G/L Rent Posting](../../03-General-Ledger/business-processes/07-Reversal-of-GL-Rent-Paid.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.3, pages 133–134.
