---
seo:
  title: List (Multi-Select) Fields | Gridfox
title: List (Multi-Select) Fields
---
# List (Multi-Select) Fields

The List (Multi-Select) Field Type can be used for assigning one or many predefined values to a Record.

For example, if you use Gridfox as a task management tool, you could add a Multi-Select List Field to tag Tasks with categories. 

Multiple tags could then be assigned to a Task.

![Multi Select List Example](/assets/images/multi-select-list-example.png "Multi Select List Example")

List (Multi-Select) Fields can be specified as a [Required Field](/building-a-project/field-settings#required-fields) for a Table but they cannot be set as a [Unique Field](/building-a-project/field-settings#unique-fields) or a [Reference Field](/building-a-project/reference-fields).

{% include tip.html content="If a Record should only have one assigned value, rather than multiple, use a [List Field](/building-a-project/list-fields) instead of a List (Multi-Select) Field." %}

## Configuring List (Multi-Select) Field Items

Once a List (Multi-Select) Field has been [added to a Table](/building-a-project/creating-fields), the items that are shown in the dropdown for this Field can be configured.

Open the Field Settings by clicking on the Field in the [Grid View Editor](/building-a-project/grid-views) or the Explorer.

Add a new option to the Field by clicking **Add List Item** and entering a name for the item. 

![Adding Multi Select List Item](/assets/images/adding-multi-select-list-item.gif "Adding Multi Select List Item")

You can rename existing List Items by changing the text for an existing option.

![Renaming Multi Select List Item](/assets/images/renaming-multi-select-list-item.gif "Renaming Multi Select List Item")

{% include tip.html content="All new List (Multi-Select) Fields that are added will have three default List Items added also." %}

To delete an existing List Item, click the delete button next to the List Item.

![Remove Multi Select List Item](/assets/images/remove-multi-select-list-item.jpg "Remove Multi Select List Item")

Any Records which had the deleted List Item selected will be updated and the deleted List Item removed.

## Specifying Default List Items

When configuring List Items for a List (Multi-Select) Field, you can optionally choose some of the values to be set as default values.

When a new Record is created, the List (Multi-Select) Field will be prepopulated with the chosen default values. The User creating the Record can amend which values are selected as required.

To specify a List Item as a default value, check the checkbox in the List Item configuration.

![Set Multi Select list Item as Default](/assets/images/set-multi-select-list-item-as-default.jpg "Set Multi Select list Item as Default")

## Colour Coding List Items

To help give your Users an at-a-glance view of data, you can colour code the List Items.

The colour coding can then be shown on your Views, including [Calendar](https://staging--gridfox.netlify.app/building-a-project/calendar-screens), [Boards](https://staging--gridfox.netlify.app/building-a-project/board-screens), [Gantt Charts](https://staging--gridfox.netlify.app/building-a-project/gantt-screens) and Dashboard [Charts](https://staging--gridfox.netlify.app/building-a-project/chart-types).

To add a colour to a List Item, click the grey square in the colour column when configuring the List Items then choose a colour.

![Colour Coding Multi Select List](/assets/images/colour-coding-multi-select-list.gif "Colour Coding Multi Select List")