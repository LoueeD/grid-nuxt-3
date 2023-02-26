---
seo:
  title: "Chart Types | Gridfox "
title: Chart Types
---
# Chart Types

There are six different types of Chart that can be added to your Dashboard, each with their own configuration and settings.

## Pie Charts

Pie Charts can be used to segment data into categories. The proportion of data in each segment can be seen at a glance.

1. Enter a Name for the Chart
2. Choose which [Table](/building-a-project/an-introduction-to-tables) the Pie Chart should show data from
3. Optionally, select a [Saved Filter](/building-a-project/saved-filters) to show a subset of data on the Chart
4. Choose which [Field](/building-a-project/an-introduction-to-fields) to Group the data by, where the Field Type must be a List, Date, Date Time, User, User Group or linked Parent
5. In 'Show Pie Chart Values', choose how segment values should be displayed

   * **Hover**: The segment values are shown when a user hovers their mouse over that segment of the Chart
   * **Always**: The segment values will be shown at all times when the Pie Chart is viewed
6. In 'Sum Results By', choose how to calculate the value of each segment

   * **Count**: Number of Records that match the grouping
   * **Sum**: Total value in a chosen Field for all Records that match the grouping, where the Field chosen is a Number, Money or Formula Field
7. Click **Save Chart**

![Creating a Pie Chart](/assets/images/creating-a-pie-chart.gif "Creating a Pie Chart")

## Number Tiles

Number Tiles display a single number based on the count of Records in a Table or the total sum of a Field on Records in a Table.

1. Enter a Name for the Number Tile
2. Choose which [Table](/building-a-project/an-introduction-to-tables) the Number Tile should show data from
3. Optionally, select a [Saved Filter](/building-a-project/saved-filters) to show a subset of data on the Chart
4. In 'Sum Results By', choose how to calculate the value shown on the Number Tile

   * **Count**: The number of Record in the selected Table that match the filter, if one has been selected
   * **Sum**: Total value in a chosen Field for all Records in the selected Table that match the filter, if one has been selected

     With this option you must choose a Field of Type Money, Number of Formula to sum by
5. Click **Save Chart**

![Creating a Number Tile](/assets/images/creating-a-number-tile.gif "Creating a Number Tile")

## Line Charts

Line Charts display data across two axes.

1. Enter a Name for the Chart
2. Choose which [Table](/building-a-project/an-introduction-to-tables) the Chart should show data from
3. Optionally, select a [Saved Filter](/building-a-project/saved-filters) to show a subset of data on the Chart
4. Choose which Field you would like to Group data by on the x-axis of the Chart, where the Field Type must be a List, Date, Date Time, User, User Group or linked Parent
5. Finally, choose how the value of each point is determined in the 'Sum Results By' section, where you can choose to from one of the following options:

   * **Count**: Number of Records that match the grouping
   * **Sum**: Total value in a chosen Field for all Records that match the grouping, where the Field chosen is a Number, Money or Formula Field
6. Click **Save Chart**

![Creating a Line Chart](/assets/images/creating-a-line-chart.gif "Creating a Line Chart")

## Bar Charts

Bar Charts display data across two axes, showing a bar for each of the x-axis values.

1. Enter a Name for the Chart
2. Choose which [Table](/building-a-project/an-introduction-to-tables) the Chart should show data from
3. Optionally, select a [Saved Filter](/building-a-project/saved-filters) to show a subset of data on the Chart
4. Choose which Field you would like to Group data by on the x-axis of the Chart, where the Field Type must be a List, Date, Date Time, User, User Group or linked Parent
5. Finally, choose how the value of each point is determined in the 'Sum Results By' section, where you can choose to from one of the following options:

   * **Count**: Number of Records that match the grouping
   * **Sum**: Total value in a chosen Field for all Records that match the grouping, where the Field chosen is a Number, Money or Formula Field
6. Click **Save Chart**

![Creating a Bar Chart](/assets/images/creating-a-bar-chart.gif "Creating a Bar Chart")

## Funnel Charts

Funnel Charts show a pipeline of data, which can be useful to show sales opportunities or project flows.

1. Enter a Name for the Chart
2. Choose which [Table](/building-a-project/an-introduction-to-tables) the Chart should show data from
3. Optionally, select a [Saved Filter](/building-a-project/saved-filters) to show a subset of data on the Chart
4. Choose which Field you would like to Group data by on the Chart, where the Field Type must be a List, Date, Date Time, User, User Group or linked Parent
5. Choose how you would like the segment values calculated, where depending on the type of data you are choosing to show on the Funnel Chart, you may wish to show a snapshot of the current state of Records or instead show all stages that a Record has been through:

   * **Historic**: Each wedge in the funnel chart is the total value of the Records which have the specified list value plus all Records with a list value following the specified list value.

     This may be useful to see the progress of a marketing campaign where the stages may be Emails Sent, Emails Opened, Meetings Scheduled, Sales Made.
   * **Current**: Each wedge in the funnel chart it the total value of the Records which match the specified list value.

     This option can be used to see a Sales Pipeline where you can see the value of Opportunities in each of the defined Stages.
6. Finally, choose how the value of each point is determined in the 'Sum Results By' section, where you can choose to from one of the following options:

   * **Count**: Number of Records that match the grouping
   * **Sum**: Total value in a chosen Field for all Records that match the grouping, where the Field chosen is a Number, Money or Formula Field
7. Click **Save Chart**

Note that if the value in a Record is negative then it will be summed with the other Records. If the overall value of a funnel wedge is negative then the negative value will be displayed.

![Creating a Funnel Chart](/assets/images/creating-a-funnel-chart.gif "Creating a Funnel Chart")

## Record Grids

Record Grids show a list of Records from a Table in the Project. You can specify a filter for the data that should be shown, which makes this component useful for showing top priority tasks or high value sales items.

1. Enter a Name for the Chart
2. Choose which [Table](/building-a-project/an-introduction-to-tables) the Chart should show data from
3. Optionally, select a [Saved Filter](/building-a-project/saved-filters) to show a subset of data on the Chart
4. Choose which Fields you would like to display on the Record Grid, noting that you can choose Fields from the select Table as well as Fields from any [linked Parent Tables](/building-a-project/table-relationship-types)
5. Click **Save Chart**

![Creating a Record Grid](/assets/images/creating-a-record-grid.gif "Creating a Record Grid")