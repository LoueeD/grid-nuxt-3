---
title: Uploading Tables from Spreadsheets
---
# Creating a Table using Spreadsheet Upload

Rather than creating each Table individually for a Project, you can create Tables and Fields in bulk by uploading a spreadsheet.

This is useful if you already have a spreadsheet containing the data that you would like to store in Gridfox.

Each of the spreadsheet worksheets will create a new Table. Within each worksheet, all columns will add Fields to the Tables. Any rows in the spreadsheets will create Records in the Tables.

### Preparing the Spreadsheet

Firstly, prepare your spreadsheet for upload:

1. Ensure each of the Tables that you would like to create are on a separate worksheet in the spreadsheet
2. Remove any charts or extraneous worksheets
3. Append Field information to column headers 

   For each column you can append values such as #Ref to set the field as a [reference field](/building-a-project/field-settings#reference-fields) or #ID to set the field as a [unique field](/building-a-project/field-settings#unique-fields). 

   To set the Field Type append the name of the Field Type e.g. #Date, #List

{% include tip.html content="If you specify a field as being a List, Gridfox will take all the unique values in that column and populate the list values for you." %}

Icon and image fields are not supported on the spreadsheet upload.

You can also add links to other tables by referencing parent tables before the field e.g. *Company.CompanyName.* For more information on parent and child tables see [Linking Tables](/building-a-project/linking-tables).

### Uploading the Spreadsheet

The spreadsheet upload tool is found in the Explorer. To navigate to the Explorer, select the **Explorer** tab in the top right hand corner of your Project.

![Table Explorer Tab](/assets/images/explorer-tab.jpg "Table Explorer Tab")

Click **Upload Spreadsheet** in the top left hand corner of the canvas.

![Upload Spreasheet Button Table Builder](/assets/images/upload-spreasheet-button-table-builder.jpg "Upload Spreasheet Button Table Builder")

Select your spreadsheet. The draft data model will display.

<img class="shadow" alt="CreateModelSpreadsheet" src="/assets/help/img/CreateModelSpreadsheet.png" />

Make any changes to the model as needed, then click **Build Data Model**. This will create the Tables and Fields. It will then insert the data from your spreadsheet as Records.