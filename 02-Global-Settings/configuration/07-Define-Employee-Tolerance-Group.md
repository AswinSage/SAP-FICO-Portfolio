# Define Tolerance Groups for Employees

## 1. Objective

Define employee tolerance limits for document amounts, open items, and permitted payment differences.

## 2. Business Purpose

Employee tolerance groups establish financial processing limits for employees. The source project describes these limits as a control over document amounts, open items, and payment differences, supporting authorization and reducing unauthorized postings.

## 3. Configuration Activity

**Configuration item:** Define Tolerance Groups for Employees

**SAP navigation:**

`SPRO → SAP Reference IMG → Financial Accounting → Financial Accounting Global Settings → Document → Tolerance Groups → Define Tolerance Groups for Employees`

**Transaction code:** Not specified in the source procedure. Record the code actually used, if applicable.

## 4. Procedure

1. Open the Define Tolerance Groups for Employees activity.
2. Select **New Entries**.
3. Enter the Tolerance Group.
4. Enter the description, if available.
5. Maintain the amount per document.
6. Maintain the amount per open item.
7. Maintain the permitted payment difference.
8. Verify all mandatory details.
9. Save the tolerance group.

## 5. Project Configuration Values

| Field | Project value |
|---|---|
| Tolerance Group | To be recorded from SAP |
| Description | To be recorded from SAP |
| Amount per document | To be recorded from SAP |
| Amount per open item | To be recorded from SAP |
| Permitted payment difference | To be recorded from SAP |

## 6. Validation

- [ ] Tolerance Group is defined.
- [ ] Description is correct, if maintained.
- [ ] Amount per document is checked.
- [ ] Amount per open item is checked.
- [ ] Permitted payment difference is checked.
- [ ] Saved values can be displayed.

## 7. Evidence

Suggested screenshot: `06-Define-Employee-Tolerance-Group.png`

## 8. Implementation Notes

Record the actual limits and the business rationale for them. Do not publish employee-specific or sensitive authorization details.

## 9. Source Note

Based on Phase 2, section 2.4, Tolerance Group of Employees, in the uploaded SAP FICO implementation project document.
