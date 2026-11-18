# Define Posting Period Variant

## 1. Objective

Define a Posting Period Variant to control the accounting periods in which financial postings are permitted.

## 2. Business Purpose

A Posting Period Variant controls which accounting periods are open or closed for financial postings. It supports posting-date control and helps prevent postings to periods that are closed.

## 3. Configuration Activity

**Configuration item:** Define Variants for Open Posting Periods

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Document → Posting Periods → Define Variants for Open Posting Periods`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Define Variants for Open Posting Periods activity.
2. Select **New Entries**.
3. Enter the four-character Posting Period Variant.
4. Enter the description.
5. Select the account type, if required by the configuration.
6. Verify the mandatory details.
7. Save the variant.

## 5. Project Configuration Values

| Field | Project value |
|---|---|
| Posting Period Variant | To be recorded from SAP |
| Description | To be recorded from SAP |
| Account Type | To be recorded from SAP, if maintained |
| Open period settings | Record from the actual configuration |

## 6. Validation

- [ ] Posting Period Variant is created.
- [ ] Identifier and description are correct.
- [ ] Account type settings are checked, where applicable.
- [ ] Required open-period controls are documented.
- [ ] Saved configuration can be displayed.

## 7. Evidence

Suggested screenshot: `05-Define-Posting-Period-Variant.png`

## 8. Implementation Notes

The source procedure describes defining the variant. Capture the actual open-period maintenance and company code assignment separately if those activities were performed in the project; do not imply they are evidenced by this definition step alone.

## 9. Source Note

Based on Phase 2, section 2.3, Posting Period Variant, in the uploaded SAP FICO implementation project document.
