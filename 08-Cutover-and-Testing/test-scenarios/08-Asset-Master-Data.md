# Test Scenario 8.8 – Asset Master Data

## Scenario Reference

| Field | Detail |
|---|---|
| Phase | 8 – Cutover Activities – Testing |
| Source section | 8.8 Asset Master Data |
| Source procedure page | 146 |
| Source screenshot pages | 147–152 |
| Scenario category | Asset master-data validation |
| Execution in current target environment | Not independently verified |

## Objective

Validate creation of single assets, group assets, and sub-assets with the required company-code, asset-class, organisational, and depreciation assignments.

## A. Single Asset

### Source Procedure

1. Enter Asset Class and Company Code.
2. Enter the Asset Description.
3. Enter Cost Centre where required.
4. Maintain Time-Dependent Data.
5. Enter Depreciation Area, Depreciation Key, and Useful Life.
6. Enter Depreciation Start Date where required.
7. Verify mandatory details and save.

### Expected Results

- Asset master is created under the correct asset class and company code.
- Asset number and subnumber are generated or assigned.
- Description and time-dependent organisational data are available.
- Depreciation area, depreciation key, useful life, and start date are consistent with the asset class and accounting policy.
- The asset master can be displayed.

## B. Group Asset

The source includes a separate Group Asset example on pages 149–150. It demonstrates asset master data in the group-asset path, including general and depreciation-related views.

### Expected Results

- Group asset master is saved with its relevant asset class and company code.
- Group asset valuation and depreciation data are maintained as required by the configured asset class.
- The resulting master record is displayable and distinguishable from a single asset record.

## C. Sub-Asset

The source identifies the Sub-Asset example on pages 151–152. The extracted text contains the subsection heading but does not provide a complete field-by-field procedure.

### Expected Results

- Sub-asset is created under the intended main asset.
- Main asset number and subnumber relationship are correct.
- Company code, asset class inheritance or assignment, and depreciation terms are consistent with the main asset and configured rules.
- Main asset and sub-asset can be displayed as related records.

The detailed sub-asset procedure is not inferred beyond the visible source scope.

## Preconditions

- Chart of Depreciation and required depreciation areas exist.
- Asset classes, account determination keys, screen layouts, and number ranges exist.
- Depreciation keys are configured and valid for the relevant depreciation area.
- Company Code and relevant Cost Centre / Profit Centre assignments are available where required.

## Validation Assertions

| Validation point | Expected condition |
|---|---|
| Asset identity | Asset number, subnumber, description and class are correct |
| Company code | Asset belongs to the intended company code |
| Organisational data | Cost Centre and time-dependent assignments are correct where applicable |
| Depreciation | Area, key, useful life and start date are consistent |
| Group asset | Group asset data is saved and displayable |
| Sub-asset | Main asset / subnumber relationship is correct |
| Display | Asset master can be displayed after creation |

## Source Screenshot Register

| PDF page | Screenshot subject |
|---:|---|
| 147–148 | Single Asset |
| 149–150 | Group Asset |
| 151–152 | Sub-Asset |

## Related Portfolio Scenarios

- [Create Single Asset Master](../../06-Asset-Accounting/business-processes/20-Create-Single-Asset-Master.md)
- [Create Group of Assets](../../06-Asset-Accounting/business-processes/21-Create-Group-of-Assets.md)
- [Create Sub-Asset](../../06-Asset-Accounting/business-processes/22-Create-Sub-Asset.md)

## Source Note

*SAP FICO Implementation Project Document*, Phase 8, section 8.8, pages 146–152. The companion *SAP FICO Business Processes* PDF also includes separate single-asset, group-of-assets and sub-asset business processes.
