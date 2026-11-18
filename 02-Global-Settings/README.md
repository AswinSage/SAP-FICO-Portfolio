# Global Settings

## 1. Overview

Global Settings establish key financial accounting controls used by company codes. The implementation project document identifies configuration activities for field status, fiscal year structure, posting periods, and employee tolerance controls.

## 2. Configuration Scope

| No. | Activity | Purpose |
|---:|---|---|
| 1 | Define Field Status Variant | Controls field entry behavior during G/L document posting |
| 2 | Assign Company Code to Field Status Variant | Applies field status controls to a company code |
| 3 | Maintain Fiscal Year Variant | Defines posting periods and special periods |
| 4 | Assign Fiscal Year Variant to Company Code | Applies the accounting calendar to a company code |
| 5 | Define Posting Period Variant | Controls open and closed posting periods |
| 6 | Define Tolerance Groups for Employees | Defines employee posting and payment-difference limits |
| 7 | Assign User Name to Tolerance Group | Applies the relevant tolerance group to a user |

## 3. Documentation Structure

| File | Description |
|---|---|
| `configuration/01-Global-Settings-Overview.md` | Configuration sequence and evidence register |
| `configuration/02-Define-Field-Status-Variant.md` | Field status variant and field status groups |
| `configuration/03-Assign-Company-Code-to-Field-Status-Variant.md` | Company code assignment |
| `configuration/04-Maintain-Fiscal-Year-Variant.md` | Fiscal year and posting period structure |
| `configuration/05-Assign-Fiscal-Year-Variant-to-Company-Code.md` | Fiscal year assignment |
| `configuration/06-Define-Posting-Period-Variant.md` | Posting period control |
| `configuration/07-Define-Employee-Tolerance-Group.md` | Employee tolerance limits |
| `configuration/08-Assign-User-to-Tolerance-Group.md` | User assignment |

## 4. Validation Approach

Each configuration activity must be checked in the SAP system and supported by a screenshot or other project evidence. Project-specific values must be copied from the actual configuration, not estimated.

## 5. Source and Scope Note

The activities in this module follow Phase 2, Global Settings, of the uploaded SAP FICO implementation project document. This folder documents the source procedures; completion status must be established from project evidence.
