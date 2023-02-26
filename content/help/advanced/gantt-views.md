---
seo:
  title: Gantt Views | Gridfox
  description: Help guide that shows Users how to configure Gantt Views for their
    Gridfox Project. Gantt Views help Users see where activities may overlap and
    their duration.
title: Gantt Views
---
# Gantt Views

Gantt Views allow you to visualize the schedule of your Records over time. It allows your Users to see at a glance where activities and tasks may overlap and how long they will take.

![Gantt View](/assets/images/gantttutorial_header-image.jpg "Gantt View")

## Creating Gantt Views

To create a new Gantt View, open up the **Create** menu in the bottom left corner and choose the **Gantt** option.

{% include tip.html content="You can use `Ctrl` + `\` to open the **Create** menu if it currently collapsed." %}

Enter a name for your new Gantt View and click the next arrow.

![Create Gantt View](/assets/images/create-gantt-view.gif "Create Gantt View")

You will then be guided through the configuration steps for your new Gantt View.

Start by choosing which Table you want to show information from on the Gantt View.

You will then be prompted to pick the Fields that should be used for the start and end dates of each block on the Gantt View.

These date fields can be from the Table you selected in the first step, or from a [linked Table](/building-a-project/linking-tables).

Finally, choose which Field should be used as the title for each block on the Gantt View. 

Click **Save** to create your new View.

![Configuring a Gantt View](/assets/images/configuring-a-gantt-view.gif "Configuring a Gantt View")

## Additional Configuration Options

Once you have chosen the core settings for your Gantt Chart, there are some additional optional steps you can take to customise your View further.

### Display Fields

To show additional information about each Record on your Gantt Chart, you can add Display Fields. These will be shown in the left hand section of the Gantt Chart.

![Gantt Display Fields](/assets/images/display-fields.jpg "Gantt Display Fields")

To configure these, click **Display Fields** in the Gantt Configuration menu.

Drag the Fields from the Available Fields section into the Display Fields section.

![Configuring Gantt Display Fields](/assets/images/gantt-display-fields.gif "Configuring Gantt Display Fields")

{% include tip.html content="To change the order of Display Fields, move them up and down the Display Field column by dragging and dropping each Field." %}

### Grouping Events

Optionally, entries on the Gantt Chart can be grouped into sections based on a [linked Parent or Grandparent Table](/building-a-project/table-relationship-types).

![Grouped Gantt Chart](/assets/images/grouped-gantt-chart.png "Grouped Gantt Chart")

To configure a grouping, click **Group Events** in the Gantt Configuration menu.

Choose a grouping option from the menu. You can then specify additional Display Fields for the groupings.

![Grouping Gantt Charts](/assets/images/grouping-gantt-charts.gif "Grouping Gantt Charts")

### Colour Coding

To help your Users understand the data on the Gantt Chart at a glance, you can optionally select to colour code the Events on the Gantt Chart.

You can choose to colour the Records based on the value in a List Field, a User Field or a User Group Field.

To configure the colour coding, click **Gantt Colours** in the Gantt Configuration menu.

Choose which Field to use for the colour coding.

![Colour Coding Gantt](/assets/images/colour-coding-gantt.gif "Colour Coding Gantt")

## Updating Gantt Views

Gantt Views can be amended at any time.

Click **Edit Current View** when you are looking at the Gantt Chart. Alternatively, open the View menu and click **Edit**.

{% include tip.html content="You can use `Ctrl` + `space` to open the View Editor." %}

Make any changes that are needed and then click the **Save** button. Changes will take effect immediately for everyone in the Project.

### Renaming a Gantt View

To change the name of one of your Gantt Views, open the Gantt Configuration and click into the name section.

Make the changes required and click **Confirm**.

![Rename Gantt View](/assets/images/renaming-gantt-view.gif "Rename Gantt View")

## Deleting Gantt Views

To delete a Gantt View, open the View Menu for the Gantt Chart and select **Delete**. Confirm the action by clicking **Delete** again.

Alternatively, select the View in the navigation panel and click **Edit Current View**.

Click the **Delete** button in the settings tray. Confirm the action by clicking **Delete** again.

![Delete Gantt View](/assets/images/delete-gantt-view_rs.gif "Delete Gantt View")

{% include note.html content="Deleting a Gantt View cannot be undone." %}