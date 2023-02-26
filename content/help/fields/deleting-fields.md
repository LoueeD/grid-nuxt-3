---
seo:
  title: Deleting Fields | Gridfox
title: Deleting Fields
---
# Deleting Fields

If there are Fields that are no longer required on a Table, they can be deleted. 

Fields can be deleted from the Table's [Grid View](/building-a-project/grid-views) or using the Explorer.

When you delete a Field all data will be removed from the Field and it will be removed from all [Views](/building-a-project/an-introduction-to-views). Additionally:

* Any [Boards](/building-a-project/board-views) which have a column grouping by this Field will show as blank screens and require reconfiguring.

  If the Field is used for row groupings, then the Board row grouping will be removed.
* Any [Saved Filters](/building-a-project/creating-screens#creating-screen-filters) which use this Field will be deleted

  Note that any Charts which use this Saved Filter will also be removed from the Dashboard View. The Chart will still show in Builder Mode to allow you to update the configuration.
* Any Charts which are configured to group data by this Field are removed from the [Dashboard View](/building-a-project/an-introduction-to-dashboards).

  Note that the Charts will show up in Builder Mode to allow you to update the configuration.

  If a [Record Grid](/building-a-project/chart-types#record-grid) Chart uses this Field as one of its columns, the column will be removed.
* The Field will be removed from any [Forms](/building-a-project/an-introduction-to-forms) which use the Field.

  The Form will remain available at its current link.

{% include tip.html content="Deleting a Field cannot be undone." %}

## Deleting a Field using the Grid View Editor

1. Navigate to the Grid View for the Table that you would like to delete a Field from
2. Expand the **Create** menu in the bottom left hand corner
3. Click **Edit Current View**
4. Drag the Field you want to delete into the **Drop Field to Delete** section

   Alternatively click **Delete Field** in the left hand side panel
5. Confirm the action by clicking **Delete**
6. Click **Save**

![Drag to Delete Field](/assets/images/drag-to-delete_rs.gif "Drag to Delete Field")

{% include note.html content="If the Field that you wish to delete is not showing on the Grid View, the Explorer can be used instead. Alternatively, you can [show the Field](/building-a-project/creating-screens#hiding-and-showing-fields) on the Grid View and then delete it from the Table." %}

## Deleting a Field using the Explorer

1. Start by selecting the **Explorer** tab in the top right hand corner
2. Click the X icon that shows to the right of the Field name

   Alternatively, click **Delete Field** in the left hand side panel
3. Confirm the action by clicking **Delete** again
4. Click **Save** to apply the change to your Project.

![Delete Field Table Builder](/assets/images/delete-field-explorer.gif "Delete Field Table Builder")