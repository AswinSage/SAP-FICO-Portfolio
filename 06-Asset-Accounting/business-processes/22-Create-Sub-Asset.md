# Process 22: Create Sub-Asset

## 1. Objective
Create an additional asset component under an existing main asset.

## 2. Business Purpose
The source describes a sub-asset as a separately tracked component linked to a main asset, with its own accounting values and depreciation details.

## 3. Process Flow
- Preceding: Asset Master
- Required: Create Sub-Asset
- Succeeding: Asset Posting

## 4. Prerequisites
**Configuration:** Chart of Depreciation, Depreciation Area, Asset Class, Account Determination Key, Screen Layout, Asset Number Range, Depreciation Key.

**Master data:** Asset Master (`AS01`); G/L Master (`FS00`).

## 5. Procedure Outline
1. Identify the existing main asset.
2. Confirm the required asset accounting configuration.
3. Create the sub-asset under the appropriate main asset reference.
4. Maintain the sub-asset description and depreciation details.
5. Save and record the sub-asset identifier.
6. Verify the main-asset/sub-asset relationship.

Source examples: Keyboard (2) and Mouse (2).

## 6. Validation and Reporting
Reports stated in source: `AW01N`, `AR01`, `S_ALR_87011964`, `S_ALR_87011990`.
- [ ] Main asset reference is correct.
- [ ] Sub-asset is separately identified.
- [ ] Depreciation details are checked.
- [ ] Asset reports display the records.

## 7. Evidence

**Source PDF screenshot pages:** 77-80 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).
Suggested: `22-Create-Sub-Asset-Keyboard.png`, `22-Create-Sub-Asset-Mouse.png`.

## 8. Implementation Notes
Record the actual parent asset and sub-asset relationship from the system.

## 9. Source Note
Business Processes document, Process 22, pages 76–80.