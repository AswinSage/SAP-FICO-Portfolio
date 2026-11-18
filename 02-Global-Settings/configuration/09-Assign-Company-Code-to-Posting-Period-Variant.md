# Assign Company Code to Posting Period Variant

## 1. Objective
Document assignment of the Posting Period Variant to the relevant company code.

## 2. Business Purpose
The source explains that the assignment applies posting period controls to a company code, determining which accounting periods are open or closed for posting.

## 3. Configuration Activity
**SAP navigation:** `SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Documents → Posting Periods → Assign Variants to Company Code`

## 4. Procedure
1. Select the required Company Code.
2. Enter the Posting Period Variant.
3. Verify the assignment.
4. Save.

## 5. Assignment Record
| Field | Project value |
|---|---|
| Company Code | Record from SAP |
| Posting Period Variant | Record from SAP |
| Assignment result | Pending verification |

## 6. Validation
- [ ] Company code exists.
- [ ] Posting Period Variant exists.
- [ ] Correct variant is assigned.
- [ ] Assignment can be displayed after saving.

## 7. Evidence
Suggested: `08-Assign-Posting-Period-Variant.png`.

## 8. Source Note
Implementation project document, Phase 2, section 2.3.1.