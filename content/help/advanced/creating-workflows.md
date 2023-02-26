---
title: Creating Workflows
---
# Creating Workflows

1. Select the **Automate** tab in the top right hand corner
2. If there are no Workflows in the Project you will be taken to a blank canvas for a new Workflow

   Otherwise, click **Create Workflow** 
3. Choose which [Table](/building-a-project/an-introduction-to-tables) that the Workflow is for
4. Enter a name for the Workflow
5. Add a [Workflow Trigger](/building-a-project/creating-workflows#workflow-trigger-types) by dragging it onto the canvas
6. Optionally add a [Workflow Condition](/building-a-project/adding-workflow-conditions)
7. Add and configure a Workflow Action of type [Send Email](/building-a-project/send-email-workflow-step), [Send Webhook](/building-a-project/send-webhook-action) or [Google Calendar Event](/building-a-project/google-calendar-event-action)

   Note that only one Action can be added to a Workflow
8. Click **Save** in the top right hand corner of the canvas

{% include note.html content="By default, all workflows are enabled and will become immediately active after saving. To change this, toggle the **Workflow Status** switch before you save." %}

## Workflow Trigger Types

Once you have selected which Table that the Workflow is taking action on, you must choose the event that triggers the workflow to start.

There are four trigger types to choose from.

| Trigger Type  | Details                                                                                        | Example                                                                            |
| ------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| Create Record | Workflow steps will trigger when a new Record for the selected Table is saved                  | Send an email to the Sales team when a new opportunity is created                  |
| Update Record | Workflow steps will trigger when a change is made to an existing Record for the selected Table | Send an email to the account owner when an account status is changed               |
| Delete Record | Workflow steps will trigger when an existing record for the specified table is deleted         | Send an email to the HR team when an employee record is deleted                    |
| Schedule      | Workflow steps will trigger on the defined schedule                                            | Send an email every week to to the operations team with their upcoming tasks to do |



### Scheduled Trigger Type

For Workflows with a trigger type of Schedule, there are some additional options to configure which determine how frequently the Workflow should run.

To access the options, add a Schedule trigger type to the canvas and click on the block. This will open the menu in the sidebar to configure the recurrence. The options are:

1. **Daily** 

   Runs every day on a chosen hour
2. **Weekly**

   Runs every week on a chosen day and at a chosen hour
3. **Monthly**

   Runs every month on a chosen date and at a chosen hour

   Note if the 29th, 30th or 31st is selected then for shorter months the Workflow will run on the last day of the month.