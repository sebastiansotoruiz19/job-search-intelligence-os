# Changelog — Job Search Intelligence OS (PL-002)

## v1.1 — Public Demonstration Edition

### Fixed
- BUG-001: Removed duplicate counting of historical Active applications.
- BUG-002: Corrected historical role-category application counts.
- BUG-003: Included historical Offers in the cumulative funnel.
- BUG-004: Added unique application counting, live status precedence and highest-stage preservation for reactivated records; updated role, source, monthly and funnel calculations.
- BUG-005: Replaced fixed status-count ranges with structured table references.
- BUG-006: Removed two obsolete named ranges containing invalid references.
- BUG-007: Replaced fixed reporting months with a rolling six-month window.
- BUG-008: Restored proportional dashboard chart scaling.
- Extended Live Data dropdown validation and conditional formatting to include the first application row.

### Improved
- Linked main response and interview KPIs to the corrected cumulative funnel.
- Updated lifecycle instructions and reactivation rules.
- Documented modern Excel compatibility requirements and reporting limitations.
- Standardized instruction spacing, date display and KPI formatting.
- Prepared fictional demonstration data with 16 unique applications, including two reactivated applications.
- Removed original job links, personal application records and local-path metadata from the public copy.

### QA
- Populated demonstration, reactivation and empty-state dashboard tests performed in Excel.
- Seven chart caches and saved calculation values checked in the release workbook.
- Six worksheets and 14 structured tables preserved; no stored worksheet formula errors detected.

## v1.0 — Initial version

- Application focus queue and historical repository.
- Application IDs, configurable lists and manual lifecycle migration.
- Formula-driven dashboard with status, funnel, role, source and monthly analytics.
