---
layout: default
title: What's New in this Release
nav_order: 2
parent: Home
---

# Version 1.3

* You can now define named groups of filter conditions called Filter Sets. Changing the active filter set for a report will change the filter conditions used when running the report. 

* Parameters and parameter values for SQL Passthrough reports are now handled like report filter conditions instead of report parameters. This means you can use existing filtering features like ask-at-runtime, expressions, is-one-of lists, and Filter Sets with SQL Passthrough reports. 

* When scheduling a report that has multiple filter sets defined, you can choose the filter set to use for each task in the schedule. This means that you can re-use the same report multiple times in a schedule with different sets of filter criteria for each. 

* Schedules have a new "Combine email attachments" option. If turned on, the scheduler will send the fewest emails possible for that schedule. For example, if a user is a recipient on 3 tasks in a schedule, they will receive a single email with 3 attachments.

* The template list now shows a preview/sample of the selected template.

* Added a new crosstab template style, SummaryFieldStyle, that only applies to the last row of each page. This allows you to apply specific styles to the summary row.

* Change % and Change Amount columns in a crosstab now support the count summary type. 

* You can now define the vertical and horizontal position of a chart legend, allowing you to place a legend above or below a chart. 

* You can now search the list of schedules by user, name, report name, or email. 

* Administrators can now search the list of users by name, email, role, or tenant.

* The manage reports dialog can now be used to update the report owner for multiple reports.

* You can now migrate multiple schedules to a new user or delete schedules from the new manage schedules dialog.

* The tab key will now enter an email address for a schedule recipient when creating a schedule.

* You can now toggle the Display real table and field names setting from the report wizards and formula editor. The default setting will still respect the current user's preference. 

## Bug Fixes

* When creating a SQL Passthrough report, the SQL input now updates as soon as the value changes, so you no longer need to click the OK button twice.

* Fixed a bug where the border style for a crosstab table header cell was not being respected under certain conditions.

* Changed cross-platform drawing library from Skia to DXGraphics. This fixes a number of spacing and sizing issues that only appeared when running in a linux container. 

* Fixed a bug where special characters in a report name caused problems if that report was used in a dashboard.

* Fixed a bug with the GetConditionValue function.

* Fixed a bug with chart fonts not getting saved properly. 

* When a chart has an advanced layout and multiple series, each series is now recreated when re-running the chart. 

* Fixed a bug with deleting an advanced layout for a chart report. 

* Fixed issue with "currently selected item" style for a number of themes.

* Tag items now have a darker font when using the Slate theme.

* Fixed a bug with user display for a selected report.

* Fixed a bug where a formula with group filters could not be copied.

* Fixed a bug where you could not download the application logs package if a crashdump.txt file existed.

* Fixed a bug where you were unable to load a report if there was a problem with the filter conditions.

* Fixed an issue with the expression editor not appearing properly in the advanced report designer.