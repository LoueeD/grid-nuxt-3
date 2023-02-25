---
seo:
  title: Importing and Exporting | Gridfox
title: Importing and Exporting
---
# Importing and Exporting

There are two options when choosing to export data from Gridfox:

1. **Export a Report**

   If you wish to share a snapshot of data with someone, you can use the report style export. This is available on [Grid Views](/gridfox-project/grid-views) and will export the on-screen view of data.
2. **Export & Import Data**

   If you want to add many Records to Gridfox, or make bulk edits to Records, you can use the Export & Import feature to do this. You will start by exporting the list of Records from the Table. You can then make any changes or additions required in the downloaded spreadsheet, and reimport the spreadsheet with the new data.

{% include tip.html content="If you don't have permission to Import or Export data, the **Import / Export** button will be disabled." %}

## Exporting a Report

To export a report of data from Gridfox, start by navigating to the [Grid View](/gridfox-project/grid-views) that you wish to export.

You can optionally [filter](/gridfox-project/filtering-records) the Grid View to show a subset of Records.

Click **Import / Export** and then select **Export a Report**.

![Export a Report](/assets/images/export-a-report.gif "Export a Report")

A spreadsheet of the columns and rows shown on screen will be downloaded.

{% include tip.html content="You cannot use this spreadsheet to import data. Use the [Export for Import](/gridfox-project/import-export#exporting-for-importing) option to do this." %}

## Exporting for Importing

You can use the import/export functionality to import new data into a Table, or to amend existing data.

Select a [View](/gridfox-project/an-introduction-to-views) which contains the data that you would like to add to or amend and click **Import / Export**.

If you are on a [Grid View](/gridfox-project/grid-views), make sure to click **Export Data for Import**.

Click **Download Template**. This will download a spreadsheet containing all the Records in the Table that the View is for.

![Export Template](/assets/images/export-template.gif "Export Template")

{% include tip.html content="The spreadsheet will have a column for each Field on the Table, but will not include Formula, Image, File and Icon Fields." %}

You can now make changes to the data in the spreadsheet. Add new Rows for any new Records that need adding.

Make sure you do not add or remove any columns in the spreadsheet to ensure the data can be reimported correctly.

Once you have made all the changes, save your spreadsheet.

Going back to Gridfox, click **Upload Spreadsheet** on the **Import / Export** modal.

![Import Spreadsheet](/assets/images/import-spreadsheet.jpg "Import Spreadsheet")

Select the spreadsheet that you saved and click **Open**.

You will see a summary of the changes and additions that the import will make to your data. Any errors will also be shown here.

![Import Spreadsheet](/assets/images/import-spreadsheet-summary.png "Import Spreadsheet")

Click **Import** and the changes will be applied to your data.

### Handling Field Types when Importing Records

To add data to some Fields, a specific format is required so that the data can be imported correctly.

If your Table has a [List (Multi-Select) Field](https://gridfox.com/building-a-project/list-multi-select-fields) or a User (Multi-Select) Field, ensure that List Items are separated by commas in the spreadsheet cell.