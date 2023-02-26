---
seo:
  title: Linking Tables | Gridfox
title: Linking Tables
---
# Linking Tables

Gridfox becomes really powerful when you start to add multiple Tables and link them together.

Linking Tables allows you to relate Records to one another, giving visibility of related data to your users.

There are [different types of relationships](/building-a-project/table-relationship-types) that you can create between Tables. They are all created in the same way, and can be created using either the View Editor or the Explorer.

{% include tip.html content="You may find it easier to create relationships between Tables using the Explorer, as this allows you to view multiple Tables at once." %}

## Linking Tables using the Grid View Editor

When you are making changes to the layout of a Grid View for a Table, you can select to add a relationship between this Table and another.

1. Navigate to the Grid View for the Table that you want to link to another
2. Open the **Create** menu in the bottom left hand corner
3. Click **Edit Current View**
4. Expand the Field Picker and drag a **Link to Table** Field onto the Grid

You will then be asked whether to link to an existing Table or create a new Table.

![Linking Tables using the Grid View Editor](/assets/images/linking-tables-using-the-grid-view-editor.gif "Linking Tables using the Grid View Editor")

### Linking to an Existing Table

1. Ensure the **Existing Table** tab is selected
2. Pick a Table from the list
3. Choose the [type of relationship](/building-a-project/table-relationship-types) for the two Tables
4. Click **Apply**
5. Click **Save**

![Linking to an existing Table using Grid View Editor](/assets/images/linking-to-an-existing-table-using-grid-view-editor.gif "Linking to an existing Table using Grid View Editor")

When your users are creating Records in these two Tables, they will now be able to link Records together via this relationship.

{% include tip.html content="You can add multiple relationships to a Table. Add another **Link to Table** Field into the Grid to add another link." %}

### Linking to a New Table

1. Ensure the **New Table** tab is selected
2. Enter a name for the new Table
3. Choose the [type of relationship](/building-a-project/table-relationship-types) for the two Tables
4. Click **Apply**
5. [Create Fields](/building-a-project/creating-fields) for the new Table
6. Click **Save**

![Linking to a new Table using Grid View Editor](/assets/images/linking-to-a-new-table-using-grid-view-editor.gif "Linking to a new Table using Grid View Editor")

When your users are creating Records in these two Tables, they will now be able to link Records together via this relationship.

{% include tip.html content="You can add multiple relationships to a Table. Add another **Link to Table** Field into the Grid to add another link." %}

## Linking Tables using the Explorer

1. Click the **Explorer** tab in the top right hand corner
2. Click the **Link** icon on the first Table
3. Click the **Link** icon on the second Table
4. Choose the [type of relationship](/building-a-project/table-relationship-types) for the two Tables
5. Click **Apply**
6. Click **Save**

![Linking tables using the Explorer](/assets/images/linking-tables-using-the-explorer.gif "Linking tables using the Explorer")

When your users are creating Records in these two Tables, they will now be able to link Records together via this relationship.

{% include tip.html content="You can add multiple relationships to a Table. Click the **Link icons** again to add another link." %}

## Required Relationships

If you create a [Parent-Child relationship](/building-a-project/table-relationship-types) between Tables, you can optionally set the relationship as required. This will mean that a child Record must be linked to a parent Record.

This can be used in cases where it does not make sense to have child Record without a parent Record. For example, if you were tracking Tasks for Projects, you may have a Tasks Table and a Projects Table where Tasks is a child Table of Projects. 

![Tasks & Projects](/assets/images/tasks-projects_rs.png "Tasks & Projects")

To avoid Users creating Tasks that are not related to any Project, you could choose to make the relationship between Tasks and Projects required. This would ensure that a Task cannot be created without selecting a parent Project.

Relationships can be set as required using either the View Editor or the Explorer.

### Required Relationships in the Grid View Editor

1. Navigate to the Grid View for either the Parent or Child Table
2. Open the **Create** menu in the bottom left hand corner
3. Click **Edit Current View**
4. Click on the link to the related Table
5. Check **Is Required** in the left hand side panel
6. Click **Save**

![Setting relationship as required in Grid View Editor](/assets/images/required-relationship-editor_rs.gif "Setting relationship as required in Grid View Editor")

### Required Relationships in the Explorer

1. Select the **Explorer** tab in the top right hand corner
2. Click the relationship arrow between the two Tables
3. Check the required relationship checkbox
4. Click **Save**

![Setting relationship as required in Explorer](/assets/images/setting-relationship-as-required-in-explorer.gif "Setting relationship as required in Explorer")