# Job Search Intelligence OS | PL-002

**Version 1.1 — Portfolio Lab | Public Demonstration Edition**

An Excel-based application lifecycle management and analytics system that transforms job-search records into operational insights. All demonstration applications are fictional.

## Business problem

Job seekers often track applications across multiple platforms without a consolidated view of current activity, historical outcomes, recruitment conversion or source performance. This workbook combines a daily focus queue with a historical analytical repository and a formula-driven dashboard.

## Features

- Application tracking with persistent application IDs and configurable dropdown lists.
- A 14-day review threshold with conditional formatting for aging applications.
- Historical outcomes and reactivation without inflating unique application counts.
- Current status precedence for live records and cumulative highest-stage reporting across live and historical records.
- Role and source performance, response rate, interview counts and recruitment funnel analytics.
- Rolling six-month application trends and historical time-to-first-progress reporting.
- Seven dashboard charts and integrated user instructions.

## Technical architecture

Six worksheets, 14 structured Excel tables and seven charts. The analytical layer uses structured references, COUNTIF, COUNTIFS, SUMPRODUCT, LET, VSTACK, FILTER, UNIQUE and XMATCH. No PivotTables or macros are required.

| Worksheet | Purpose | Visibility |
|---|---|---|
| Dashboard | KPIs and analytical visualization | Visible |
| Live Data | Current application focus queue | Visible |
| Historical Data | Application history and outcomes | Visible |
| Instructions | Workflow and business rules | Visible |
| Processing | Formula-driven analytical summaries | Hidden |
| Settings | Configurable lists and parameters | Visible |

## Getting started

1. Download `Job_Search_Intelligence_OS_v1.1_Demo.xlsx` from this repository.
2. Open in Microsoft 365 desktop Excel or Excel 2024 with support for the modern functions listed above.
3. Read the Instructions worksheet and review Settings.
4. Explore the fictional records, then clear application table contents in a separate working copy if starting your own tracker. Preserve headers, tables and validation rules.
5. Use the next Application ID as a fixed value when adding an application; update existing historical records by ID rather than creating duplicate history rows.
6. Preserve the original ID, application date, role category and source when reactivating applications. Keep the highest stage and first-progress date in the historical record.

## Demonstration QA

| Metric | Saved demonstration result |
|---|---:|
| Physical records | 18 |
| Unique applications | 16 |
| Response rate | 81.25% |
| Interviews reached | 8 |
| Active | 11 |
| Ghosted | 1 |
| Rejected | 3 |
| Hired | 1 |
| Offers | 2 |
| Average days to first progress | 3 |
| Next Application ID | APLI-0017 |

Manual Excel tests covered populated data, reactivation from a lower stage, duplicate-ID handling across tables, empty-state dashboard behavior and chart scaling. The release file was inspected for saved formula errors, cached chart values, validation ranges and residual original application data.

## Limitations

- The workbook assumes one record per Application ID in each table, with consistent original date, role category and source across reactivations. It is not a full event-by-event audit log.
- Recruitment stages are treated as an ordered cumulative funnel; reaching a later stage implies reaching earlier levels for reporting purposes.
- Time to First Progress uses historical records with recorded progress dates; it does not measure all live applications. Zero in the empty state means no measured progress data.
- Monthly trends show the current month and five preceding months, so demonstration results will change with the calendar date.
- The 14-day aging threshold is a review signal, not an automatic rejection or ghosting decision. The migration workflow is manual.
- Compatibility with older Excel releases and other spreadsheet applications has not been established.

## Version history

See [CHANGELOG.md](CHANGELOG.md).

## Product Preview

### Dashboard
![Dashboard](Screenshots/PL-002%20Dashboard.png)

### Live Data
![Live Data](Screenshots/PL-002%20Live%20Data.png)

### Historical Data
![Historical Data](Screenshots/PL-002%20Historical.png)

## Author

Portfolio Lab — [GitHub profile](https://github.com/sebastiansotoruiz19)
