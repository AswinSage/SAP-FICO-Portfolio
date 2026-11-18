# Process 21: Create Asset Master Data – Group of Assets

## 1. Objective
Create multiple asset master records belonging to the same asset category.

## 2. Business Purpose
The source explains that group assets share an asset class but retain individual asset numbers, acquisition values, depreciation, and book values.

## 3. Process Flow
- Preceding: G/L Master Data
- Required: Create Asset Master Data – Group of Assets
- Succeeding: Asset Posting

## 4. Prerequisites
**Configuration:** Chart of Depreciation, Depreciation Area, Asset Class, Account Determination Key, Screen Layout, Asset Number Range, Depreciation Key.

**Master data:** Asset Master (`AS01`); G/L Master (`FS00`).

## 5. Procedure Outline
1. Confirm the asset accounting configuration and required G/L master data.
2. Identify the asset category and common asset class.
3. Create each individual asset master record.
4. Maintain separate identification and relevant asset details for each record.
5. Save each asset and record its individual asset number.
6. Verify the individual records and common classification.

## 6. Validation and Reporting
Reports stated in source: Asset Explorer (`AW01N`), Asset List (`AR01`), Asset Balances (`S_ALR_87011964`), Asset History Sheet (`S_ALR_87011990`).
- [ ] Each asset has its own asset number.
- [ ] Asset class is correct.
- [ ] Individual depreciation terms and values are checked.
- [ ] Asset reports display the records.

## 7. Evidence
Suggested: `21-Create-Group-of-Assets.png`.

## 8. Implementation Notes
Record the number of assets actually created and the class used. Do not imply a single collective asset master.

## 9. Source Note
Business Processes document, Process 21, pages 73–75.