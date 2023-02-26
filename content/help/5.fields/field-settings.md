---
seo:
  title: Field Settings | Gridfox
title: Field Settings
---
# Field Settings

Once you have [created Fields](/building-a-project/creating-fields) for a Table, there are some additional settings that you can choose to use to help customize your Project.

Some of these settings apply to multiple Field Types and some are only applicable for a specific Field Type.

Field Settings can be configured in either the View Editor or the Explorer. Then click the Field that you would like to amend to open the left hand settings panel for the Field.

## Unique Fields

You can specify that a Field must contain unique values. For example, a registration number field on a vehicles Table would be set as **Is Unique**.

![Is Unique Setting](/assets/images/is-unique-setting_rs.jpg "Is Unique Setting")

If you set an existing Field to be unique, Gridfox will check that there are no existing duplicate values in the system. You may have to update your data before you can set a Field as unique.

### Ignoring Capitalisation

When a Project Admin is configuring the settings for a Text Field that must contain unique values, they can decide whether the Field’s uniqueness is case sensitive or not. 

This can be configured via the checkbox labelled Ignore Capitalisation. 

If the Ignore Capitalisation checkbox is checked, Users will not be able to save a Record with the same text value in the Field as another Record, even if the capitalisation for the test value is different.

For example, the email addresses **Joe@gridfox.com** and **joe@gridfox.com** are considered the same value when ignoring capitalisation is selected. In this example, only one Record will be created. 

By default new fields **will not** have case sensitive uniqueness.

{% include note.html content="this option is not available for Rich Text or Text Area Fields" %}

## Required Fields

You can set a Field to be required for a Table. This will validate that when a Record is created, by either direct Record creation, via [Form submission](/building-a-project/an-introduction-to-forms) or through importing Records via a spreadsheet, that the Field is populated.

![Is Required Setting](/assets/images/is-required-setting_rs.jpg "Is Required Setting")

If you set an existing Field to be required, Gridfox will not check that existing Records contain a value. When your users edit an existing Record after a field has been set as Is Required then they will not be able to save changes to the Record without a value in the required Field.

If the Field has been used on a [Form](/building-a-project/an-introduction-to-forms), it will automatically be set to required on the Form also.

## User Fields

### Setting Default User Values

You can configure a User Field to default to the currently logged in user when a new Record is created.

Tick the checkbox for **Default to currently signed in user**.

![User Setting](/assets/images/user-default-setting_rs.jpg "User Setting")

All new Records that are created will have this Field set to the User that created the Record. The User can change the value in this Field before saving the Record.

## Date Fields

### Setting Default Date Values

You can configure date fields to have a default value of today when a record is created.

Tick the checkbox for **Default to today’s date**.

![Date Default Setting](/assets/images/date-default-setting_rs.jpg "Date Default Setting")

All new Records that are created will have this Field set to the current date. The User can change the value in this Field before saving the Record.