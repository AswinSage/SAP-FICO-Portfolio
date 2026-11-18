# Test Case Register

## 1. Purpose
This register tracks validation scenarios across the SAP FICO portfolio. All cases begin as Not Executed until actual SAP evidence is attached.

## 2. Test Register

| Test ID | Area | Scenario | Expected result | Status |
|---|---|---|---|---|
| TC-GL-001 | G/L | Create/display G/L master | G/L master exists with correct company code and control data | Not Executed |
| TC-GL-002 | G/L | Direct G/L posting | Accounting document posts and balances | Not Executed |
| TC-GL-003 | G/L | Block G/L at Chart of Accounts level | Posting restriction is reflected at the intended level | Not Executed |
| TC-GL-004 | G/L | Unblock G/L at Chart of Accounts level | Restriction is removed | Not Executed |
| TC-GL-005 | G/L | Block G/L at company code level | Company-code-level restriction is reflected | Not Executed |
| TC-GL-006 | G/L | Unblock G/L at company code level | Restriction is removed | Not Executed |
| TC-GL-007 | G/L | Reverse rent posting | Reversal document offsets original document | Not Executed |
| TC-GL-008 | G/L | G/L line-item report | Selected account line items are displayed | Not Executed |
| TC-AP-001 | AP | Create vendor master | Vendor master is saved with required company code data | Not Executed |
| TC-AP-002 | AP | Create vendor reconciliation account | Vendor reconciliation account is available for assignment | Not Executed |
| TC-AP-003 | AP | Post vendor rent invoice | Vendor liability and expense are recorded | Not Executed |
| TC-AP-004 | AP | Vendor partial payment | Partial payment is reflected and remaining open item is correct | Not Executed |
| TC-AP-005 | AP | Vendor residual payment | Original item and residual open item reflect the chosen clearing method | Not Executed |
| TC-AP-006 | AP | Vendor line-item report | Vendor postings and open/cleared status are displayed | Not Executed |
| TC-AR-001 | AR | Create customer master | Customer master is saved with required company code data | Not Executed |
| TC-AR-002 | AR | Block customer | Customer block is maintained at the intended level | Not Executed |
| TC-AR-003 | AR | Unblock customer | Customer block is removed | Not Executed |
| TC-AR-004 | AR | Post customer invoice | Customer receivable and revenue are recorded | Not Executed |
| TC-AR-005 | AR | Customer payment | Payment and clearing status are reflected correctly | Not Executed |
| TC-AR-006 | AR | Customer line-item report | Customer invoices, payments, and open/cleared items are displayed | Not Executed |
| TC-AA-001 | AA | Create single asset master | Asset master is saved with required depreciation terms | Not Executed |
| TC-AA-002 | AA | Create group of assets | Individual asset records and numbers are available | Not Executed |
| TC-AA-003 | AA | Create sub-asset | Sub-asset is linked to the correct main asset | Not Executed |
| TC-AA-004 | AA | Asset acquisition | Acquisition posting updates asset values and relevant G/L accounts | Not Executed |
| TC-CO-001 | CO | Create primary cost element | Primary cost element is available with corresponding G/L account | Not Executed |
| TC-CO-002 | CO | Create secondary cost element | Secondary cost element is available for internal allocation | Not Executed |
| TC-CO-003 | CO | Create internal order | Internal Order is saved and can collect costs | Not Executed |
| TC-CO-004 | CO | Create cost centre | Cost Centre is saved with intended organizational assignments | Not Executed |
| TC-CO-005 | CO | Create profit centre | Profit Centre is saved and available for assignment | Not Executed |

## 3. Updating the Register
After each test, update the status and link the relevant evidence file. Do not change a test to Passed based only on a procedure document or screenshot of a configuration screen.