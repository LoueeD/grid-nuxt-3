---
seo:
  title: Reference Fields | Gridfox
title: Reference Fields
---
# Reference Fields

For every [Table](/building-a-project/an-introduction-to-tables) that you create, one of the Fields in the Table must be set as the Table Reference Field. The Reference Field contains the unique identifiers for each Record in the Table.

For example, you may have a Table called Projects where each Project has a Name. You can set the Name Field to be the Reference Field for Projects. This means that every Project must have a Name specified and each must have a different Name.

This will allow you to identify exactly which Record in the Projects Table is which as every Record will have a different Name.

![Project Table with Name Reference](/assets/images/project-name.jpg "Project Table with Name Reference")

Reference Fields are important when you start [creating relationships](/building-a-project/linking-tables) between Tables.

To continue the example above, the Projects Table could have a [linked](/building-a-project/linking-tables) child Table called Tasks where one Project has many child Tasks.

![Table Builder showing Projects and Tasks](/assets/images/project-and-tasks-table.jpg "Table Builder showing Projects and Tasks")

When you are creating a Task and choosing which Project to link it to, you will choose from a list of Project Names since the Name Field was set as the Reference Field.

![Project field on Task](/assets/images/project-on-task.jpg "Project field on Task")

If instead you had selected the Start Date Field to be the Project Reference Field, a list of dates would be shown in the Project list.

## How to Choose a Reference Field

The ideal Reference Field for a Table is one where:

* A Value will always be specified for all Records i.e. it is a Required Field
* Each Value will always be different for all Records i.e. it is a Unique Field

The [Field Types](/building-a-project/field-types) that can be set as a Reference Field are: Text, Text Area, Rich Text, Number, Money, Date, Date Time, Auto Counter, and URL.

For each of your Tables, look through each of the Fields which match one of the above Types and determine if every Record in the Table will have a unique value set for all Records.

If there are no Fields which are unique and required on the Table, then you can add an Auto Counter Field. This will create a sequence of numbers for each Record in the Table which will always be unique and always be set. You can then add an [ID Mask](/building-a-project/id-masks) to the Reference Field so that it is easier for your Users to identify the Record.

## Specifying a Reference Field for a New Table

Once you have [created a new Table](/building-a-project/creating-tables), before you can save the Table you must specify a Reference Field.

You can specify the Reference Field for a Table using either the View Editor or the Explorer. Select **Edit Current View** or click the **Explorer** tab, then click on the Field to open up the left hand configuration panel. Check the **Is Reference** checkbox.

![Set Reference Field Screen Editor](/assets/images/reference-field-editor_rs.jpg "Set Reference Field Screen Editor")

You can then save the Table.

{% include note.html content="Setting the Field as the Reference Field automatically sets it as **[Is Unique](/building-a-project/field-settings#unique-fields)** and **[Is Required](/building-a-project/field-settings#required-fields)**. You cannot uncheck these for the Reference Field." %}

If you haven't chosen a Reference Field for a new Table, when you click **Save** you will be prompted to select a Reference Field. You can choose an existing field or alternatively, you can click the **Add new Auto Counter Field** option which will create a new Auto Counter Field on the Table and set it as the Reference Field. Use this option if none of the existing Fields are suitable as a Reference Field.

### Changing the Reference Field for an Existing Table

The Reference Field for a Table can be changed at any time. You will need to ensure that all existing Records in your Table have a value set in the new Reference Field.

To change the Reference Field for a Table, repeat the steps above to check the **Is Reference** checkbox for the Field. This will swap the Reference Field from the previously selected Field to the new Field.

{% include tip.html content="When a new Reference Field is selected, the old Reference Field will remain unique and required. To change this, open the Field Configuration for the old Reference Field and uncheck the **Is Required** and **Is Unique** options as needed." %}