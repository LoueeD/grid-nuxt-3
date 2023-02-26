---
seo:
  title: Google Calendar Event Action | Gridfox
title: Google Calendar Event Action
---
# Google Calendar Event Action

Using the 'Google Calendar' Workflow Action, you can send event invites using data from your Gridfox Records.

{% include note.html content="The 'Google Calendar' Action can only be used in Workflows that are triggered by the create or update of a Record." %}

## Adding a Google Calendar Event Action

Start by opening up the Workflow that you would like to add a 'Google Calendar' Action to, or [create a new Workflow](/building-a-project/creating-workflows).

Drag the 'Google Calendar' block onto the canvas and click the block to open the configuration panel.

![Add Google Calendar Event](/assets/images/add-google-calendar-action_rs.gif "Add Google Calendar Event")

### Connecting to your Google Account

To allow Gridfox to create events on your calendar, you must first connect to your Google Account.

Click the **Sign in with Google** button to start connecting to a new account.

![Connect to Google](/assets/images/connect-to-google_rs.jpg "Connect to Google")

Follow the on screen steps to give Gridfox permission to create events in your calendar.

{% include tip.html content="Once you have granted Gridfox permission to link to your Google Calendar, you will be able to select this Google Account when you are creating other Workflows." %}

### Selecting your Calendar

Now choose which calendar you would like to create the events on. You can select from any Google calendar that you have 'write' permissions for.

### Specifying Event Information

Finally, specify the information about the events.

For the Event Summary and Description, you have two options for specifying these:

1. **Field**

   Select a Field from the Table, a Parent Table or a Grandparent Table that the Workflow is for.

   For example, if you are sending Events when a new Meeting is created and you have a 'Title' Field on your Meeting Table, you can select the 'Title' to be the Summary for the Google Calendar Event.
2. **Dynamic**

   Build a dynamic string of text, including Fields from the Table. Field names should be enclosed in square brackets. 

   Fields from Parent and Grandparent Tables can be included by including the singular Table Name before the Field Name.

Choose which Fields to use for the Start and End dates of the Event.

To add attendees to the Event, either:

1. Choose a set list of Users or Groups that the invite should go to
2. Choose the attendee(s) to be the User(s) in a User or Group Field on the Record which triggered the Workflow

Click **Apply** to confirm the configuration and then click **Save** to save the Workflow.

When this Workflow runs, Events will be added to the selected Google Calendar with the specified information and defined attendees.