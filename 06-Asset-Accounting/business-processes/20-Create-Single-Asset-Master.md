# Process 20: Create Asset Master Data – Single

## 1. Objective

Document creation of an individual fixed asset master record.

## 2. Business Purpose

The source describes asset master data as containing the asset class, depreciation terms, useful life, and organizational assignments required to identify and track an asset. The asset master is created before acquisition, depreciation, transfer, or retirement transactions.

## 3. Process Flow

- Preceding process: G/L Master Data
- Required process: Create Asset Master Data
- Succeeding process: Posting

## 4. Prerequisites

**Configuration required**
- Chart of Depreciation
- Depreciation Area
- Asset Class
- Account Determination Key
- Screen Layout
- Asset Number Range
- Depreciation Key

**Master data**
- G/L Master Data (`FS00`)
- Asset Master (`AS01`)

## 5. Procedure Outline

1. Confirm that the required asset accounting configuration and G/L accounts are available.
2. Open asset master creation using `AS01`.
3. Enter the asset class and required organizational details.
4. Maintain the asset description and relevant master data.
5. Maintain depreciation terms and useful-life information as required.
6. Save the asset master and record its asset number.
7. Display the asset master to verify the saved details.

The business-process PDF (SRC-02, Process 20) uses **Xerox Machine** as its single-asset example.

The implementation report (SRC-01) separately shows a Printout Machine asset master on PDF page 107:

| Field | Value visible in screenshot |
|---|---|
| Asset number / subnumber | 2 / 0 |
| Asset class | HM11 |
| Description | Printout Machine |
| Asset class description | Machine |
| Company Code | HM11 |
| Account Determination | HM11 - Machine |
| Business Area | HM21 |
| Location shown | Chennai |
| Time-dependent validity | 01.01.1900 to 31.12.9999 |
| Cost Centre | No value visible |

These are two different source examples; do not treat the Xerox Machine process scenario and Printout Machine master screenshot as the same record. Verify the asset number and organizational assignments in the target SAP system.

## 6. Validation and Reporting

**Reports stated in source**
- Asset Explorer — `AW01N`
- Asset List — `AR01`

- [ ] Asset master is created.
- [ ] Asset class and organizational assignment are checked.
- [ ] Depreciation terms are maintained.
- [ ] Asset number is recorded.
- [ ] Asset can be displayed in Asset Explorer and Asset List.

## 7. Evidence

**Source PDF screenshot pages:** 71-72 in *SAP FICO BUSINESS PROCESSES (1).pdf*. See the [Screenshot Page Index](../../00-Project-Overview/Screenshot-Page-Index.md).

`20-Create-Single-Asset-Xerox.png`.

## 8. Implementation Notes

Record the actual asset class, asset number, useful life, depreciation key, and company code. Redact sensitive asset details before publication.

## 9. Source Note

Business Processes document, Process 20, pages 69–72.