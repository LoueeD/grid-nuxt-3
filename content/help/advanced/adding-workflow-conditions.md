---
seo:
  title: Adding Workflow Conditions | Gridfox
title: Adding Workflow Conditions
---
# Adding Workflow Conditions

After [creating a new Workflow](/building-a-project/creating-workflows) then specifying the Table and trigger type, you can define the steps that are carried out after the Workflow has been triggered.

Firstly, the Workflow Conditions can be specified. This is an optional step that limits when a Workflow action will be taken. For example, you may wish to send an alert to the Delivery team when an Order has been updated to 'Ready to Ship'. This would be achieved by creating a Workflow for Order that has a trigger type of Update Record and then adding a Workflow Condition to proceed only if the Order Status Field is updated to 'Ready to Ship'.

Once the Conditions have been specified, you can then configure the Actions that are taken.

## Workflow Conditions

You can limit which Records that a Workflow carries out the defined Workflow Actions on by using a Workflow Condition.

Workflow Conditions can be added to Workflows where the trigger type is Create Record, Update Record or Schedule.

Workflow Conditions cannot be added to Workflows where the trigger type is Delete Record.

{% include tip.html content="A Workflow can have only one Workflow Condition specified." %}

For Workflows with trigger types of Create Record or Update Record, a Workflow Conditions can be defined as one of the following options:

* When a User Field on the Workflow Table matches a specified User
* When a List Field on the Workflow Table matches a specified list item

For example, you may wish to send an email to the Sales Director when a new Opportunity is created where the Opportunity Priority is set as 'High'. This would be achieved by adding a Workflow Condition to a Create Record Workflow.

For Workflows with a trigger type of Scheduled, a Workflow Condition is defined by using a [Saved Filter](/building-a-project/creating-screens#creating-screen-filters). This filter must include the Records that you wish the Workflow Action to be taken on.

For example, you may wish to send an email each week to all team members with a list of their outstanding Tasks. This would be achieved by [creating a filter](/building-a-project/creating-screens#creating-screen-filters) for Tasks where the Status is To Do and then choosing this filter as a Workflow Condition on a Schedule Workflow.

### Adding a Workflow Condition to a Create Record Workflow

Start by [creating a new Workflow](/building-a-project/creating-workflows) and adding a Create Record trigger type block. Alternatively, open up an existing Workflow.

![Workflow canvas with create record trigger added](/assets/images/create-workflow-step.jpg "Create Record Workflow")

To add a Condition to the Workflow, drag the Filter Records block onto the canvas. Click on the block to open the filter settings.

![Adding Filter Records block to workflow canvas](/assets/images/add-filter-records-create-workflow.gif "Add Filter Records block for Create Workflow")

In the filter settings menu, all User and List Fields for the Workflow Table will be listed.

If you would like the Workflow Action to only be taken when a Record is created where the selected User Field matches a specified User, select the User Field in the menu and then choose a User from the list. This will list all Users who are currently invited to the Project. Click **Apply** to confirm the settings.

![Create Workflow Filter Records settings for User field](/assets/images/create-workflow-user-filter.jpg "Create Workflow User Field filter")

Alternatively, if you would like the Workflow Action to only be taken when a Record is created where the selected List Field matches a specified list item, select the List Field in the menu and then choose a list value. Click **Apply**. 

![Create Workflow Filter Records settings for List field](/assets/images/create-workflow-list-filter.jpg "Create Workflow List Field filter")

You can now add the Workflow Actions to your Workflow.

{% include tip.html content="If you had set up a Workflow with just a Trigger and an Action, you can add a Condition at a later date by dragging and dropping the Filter Records block onto the canvas." %}

### Adding a Workflow Condition to a Update Record Workflow

The steps to add a Condition to a Workflow that has a trigger type of Update Record are the same as the steps to add a Condition to a Workflow that has a trigger type of Create Record, as detailed above.

### Adding a Workflow Condition to a Scheduled Workflow

Workflows with a trigger type of Schedule use Saved Filters as the Workflow Conditions. Before configuring the Workflow, ensure you have created a [Saved Filter](/building-a-project/creating-screens#creating-screen-filters) which covers all Records that you would like the Workflow Action to be taken on.

Start by [creating a new Workflow](/building-a-project/creating-workflows) and adding a Schedule trigger type block. Alternatively, open up an existing Workflow.

![Workflow with Schedule Step on canvas](/assets/images/schedule-workflow-step.jpg "Schedule Workflow")

To add a Condition to the Workflow, drag the Filter Records block onto the canvas. Click on the block to open the filter settings.

![Adding Filter Records block to workflow canvas](/assets/images/add-filter-records-schedule-workflow.gif "Add Filter Records block for Schedule Workflow")

Choose the Saved Filter from the menu and click **Apply**. 

You can now add the Workflow Actions to your Workflow.