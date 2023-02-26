---
seo:
  title: File Fields | Gridfox
title: File Fields
---
# File Fields

A File Field allows you to upload one or more files directly to a Record in Gridfox.

File Fields are [created](/building-a-project/creating-fields) in the same way as all other [Field Types](/building-a-project/field-types).

{% include note.html content="A File Field can be set as required, but cannot be set as a reference field or that it must contain unique values." %}

## Supported File Types

When a File Field has been added to a Table, users will be able to upload files in this Field of any of the following types:

`.xlsx` `.doc` `.docx` `.ppt` `.pptx` `.png` `.jpg` `.jpeg` `.gif` `.bmp` `.pdf` `.pages`

The maximum file size for an individual file in a File Field is 10MB.

You cannot have duplicate file names within a File Field.

## File Field Settings

You can specify how many files can uploaded for a specific File Field.

After opening the Field Configuration for a File Field in either the Grid View Editor or the Table Explorer, select the required number in the **Maximum Number of Files** setting.

![File Field Setting](/assets/images/file-field-setting_rs.jpg "File Field Setting")

{% include tip.html content="If you decrease the number of files allowed in a File Field, any Records with more files that the new limit will not be able to be saved until files are removed." %}

## Deleting a File Field

When a File Field is [deleted](/building-a-project/deleting-fields), all files in the Field are also deleted. Make sure to save a copy of any files that you need before removing a File Field.

{% include note.html content="Deleting a Field cannot be undone." %}