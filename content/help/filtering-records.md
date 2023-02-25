---
seo:
  title: Filtering Records | Gridfox
title: Filtering Records
---
# Filtering Records

To help you see only the Records you are interested in, you can apply filters to a [View](/gridfox-project/an-introduction-to-views). Filters can have multiple filter conditions to allow you to be more granular with your search.

A filter condition can have several parts. You will always start by selecting the Field that you are filtering on. The next step is to choose what that Field should contain. Some Fields have advanced options which allow you to use different operators to return the results you need. For example you can choose to show Records which have a date before a specified date. Any operators will be shown within the filter condition.

## Filtering a View

Open up the View[](/gridfox-project/an-introduction-to-views) that you would like to filter.

1. Click **Filter** in the top right hand corner
2. Click to add a new filter condition
3. Select the Field that you want to filter on and the value that Field should have
4. Repeat steps 2 and 3 until you have added all the conditions that you require
5. Click **Apply**

The View[](/gridfox-project/an-introduction-to-views) will then be filtered to show all records which match the conditions you have entered. If you have added multiple conditions, then Records will show if they match all of the filter conditions.

![Filtering Records](/assets/images/filtering-records.gif "Filtering Records")

## Clearing a Filter

Once you are finished with your filter, to see all the Records again you can clear the filter from the View.

1. Click **Filter** to open the filter panel
2. Click **Clear**

![Clearing a Filter](/assets/images/clearing-a-filter.gif "Clearing a Filter")

{% include note.html content="If you want to remove an individual filter condition rather than the entire filter, you can do this by clicking the bin icon to the right of the condition that you would like to remove." %}

## Text Based Field Filtering

When filtering by a text field, Records will be returned where they contain the text that you enter. For example, searching for 'Grid' in a Company Name Field would return 'Gridfox', and searching for 'Fox' would also return 'Gridfox'.

If you want to see all Records which have a value set in a specific Text Field, you can enter `*` in the value section of the filter condition. This can be used on all text based Field Types: Text, Text Area, Rich Text and URL.

## Number Based Field Filtering

There are several operators available for filter conditions on Fields which contain numeric values: Number, Money, Percentage and Auto Counters.

Choose whether to show Records with values equal to, greater than, less than, or between the values that you enter. You can use the operator section in the filter condition to specify this.

![Number Field Filtering](/assets/images/number-field-filtering.gif "Number Field Filtering")

## Date Based Field Filtering

There are four operators available for Date or Date Time Fields:

* **Is** - Returns values exactly equal to the date or date time that you choose
* **Is Before** - Returns values before the date or date time that you choose
* **Is After** - Returns values after the date or date time that you choose
* **Is Between** - Returns value which are after the first date or date time and before the second date or date time that you choose

Additionally, when filtering by a Date Field, you can choose to find Records with dates relative to the current date. Choose the 'Is Relative' option in the operator list. The following relative dates are available:

| **Option**    | **Description**                                                           |
| ------------- | ------------------------------------------------------------------------- |
| Next 7 Days   | Values on or before 7 days from today, inclusive of today                 |
| Next 30 Days  | Values on or before 30 days from today, inclusive of today                |
| Last 7 Days   | Values between 7 days before today and today, inclusive of today          |
| Last 30 Days  | Values between 30 days before today and today, inclusive of today         |
| Current Week  | Values within the current calendar week, where each week starts on Monday |
| Current Month | Values within the current calendar month                                  |
| Before Today  | Values before today, exclusive of today                                   |
| Today         | Values equal to today                                                     |
| After Today   | Values after today, exclusive of today                                    |

## User Field Filtering

To see which Records are assigned to a certain individual, you can pick their name from the list when filtering by a User Field. Alternatively, to show all Records which have your own name in the User Field you can use the `@Me` option.

![Filtering by a User Field](/assets/images/user-field-filtering.gif "Filtering by a User Field")

## Multi-Select List Field Filtering

There are three operators available when filtering on a Multi-Select List Field:

* **Has any of** - Returns Records which have at least one of the List Items that you choose
* **Is exactly** - Returns Records which have exactly the List Items that you choose
* **Is unset** - Returns Records which have nothing selected in the Field

## Filtering on Related Tables

In some cases, you will be able to filter on Fields from [linked Records](/gridfox-project/linked-records).

If you select a related Table in the Filter dropdown, there will then be an additional dropdown from which to select the Field from that related Table. For example, you could filter the list of Tasks by the Project Status where Projects are linked to Tasks.

![Filtering on related Tables](/assets/images/filtering-on-related-tables.gif "Filtering on related Tables")

## Using Saved Filters

Project Admins can save Filters for you to use as a way of providing shortcuts to the sections of data that you may need. Saved Filters are shown in the left hand navigation bar underneath the relevant View that they are filtering.

![Navigating to Saved Filters](/assets/images/navigating-to-saved-filters.gif "Navigating to Saved Filters")