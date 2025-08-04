---
layout: default
title: What's New in this Release
nav_order: 2
parent: Home
---

# Version 1.4

* A new "Ignore by Default" setting is available for ask-at-runtime [filter conditions]({% link _docs/creating-reports/filtering/including-records.md %}). If turned on for a filter condition, it will be automatically ignored when prompting for values. This is useful if you want to add a set of pre-defined filter conditions for a report that aren't normally part of the query, but are still handy if you need to further refine the results.

* If a report has more than one filter set defined, you are now prompted for which filter set to use when [previewing]({% link _docs/creating-reports/previewing.md %}) the report. 

* A new [Export All Reports]({% link _docs/creating-reports/importing-and-exporting-reports.md %}) button can be used to generate a zip file containing all reports. 

* Scheduled emails sent with the [Combine Email Attachments]({% link _docs/configuration/scheduling.md %}) option now support using a Horizon Reports role as a recipient. Any users in that role that have email addresses defined will be considered valid recipients when sending schedules.

* Excel data only output types now support [conditional formats]({% link _docs/creating-reports/quick-reports/step2.md %}) for font and color. 

* [Scheduled tasks]({% link _docs/configuration/scheduling.md %}) are more resiliant. If a report failure occurs during a schedule run, the schedule will now continue with the remaining reports, rather than halting. 

* When entering email addresses for a scheduled task, you can now use the space and semicolon keys to denote the end of an address in addition to the previously supported comma.

* Expressions for "Send to database" [formulas]({% link _docs/creating-reports/formulas.md %}) are no longer processed in any way. This opens up the ability to send native expressions to the database engine that previously might not have been recognized by Horizon Report's generic SQL Parser. 

* You can now open an [advanced layout]({% link _docs/creating-reports/advanced-layout-designer/index.md %}) containing a chart control with a configuration issue so it can be fixed. 

* [Crosstab templates]({% link _docs/creating-reports/templates.md %}) now support the GroupFooterSummaryFieldStyle. This can be used to apply specific styling to the subtotal lines that result from having multiple row fields.

## Bug Fixes

* Fixed an issue with Batch reports not being eligible for direct sending via email.

* Fixed an issue with the defined separator character not being used when outputting to a data only delimited format.

* Fixed an issue with the percent of total calculating not being accurate on a summary report.

* Fixed a top margin spacing issue for crosstab reports with embedded subreports.

* Fixed an issue with the alignment of a style in a Crosstab not being applied.

* Fixed an issue with the Active Directory Auth setting not being persisted.

* Fixed an issue with the save button being available for built in roles.

* Fixed an error that would rarely appear when navigating back to the Report Explorer from a wizard.

* Fixed an issue that would cause tenant membership to not be registered properly when calculating access rights.

* Fixed an issue where the Advanced Report Properties dialog would not work for passthrough reports. 

* Fixed an issue with filter sets not working for SQL Passthrough reports. 

* Fixed a bug where a Pivot control in an advanced layout would be assigned the wrong data source. 

* Fixed an issue that caused the missing virtual table error to appear multiple times when editing a report that has this problem.

* Fixed a bug that occurred when editing the Crosstab Standard Unicode template. 

* Fixed an issue that would occur when you try to delete more than one report at a time from the Manage Reports interface.