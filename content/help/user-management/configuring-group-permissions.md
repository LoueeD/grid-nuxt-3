---
seo:
  title: Configuring Group Permissions | Gridfox
title: Configuring Group Permissions
---
# Configuring Group Permissions

To control the data that your Users have access to within a Project, you put each User in a Group where the Group has a set of associated permissions.

For each Table within your Project you can specify if a User should be able to have permission to:

* **View and Amend Records in a Table**

  For each [Table](/building-a-project/an-introduction-to-tables) in the Project, you can specify whether Users in the Group can do one or many of the following: view Records, create new Records, edit existing Records, delete existing Records.
* **Import and Export Records in a Table**

  For each Table in the Project, you can specify whether Users in the Group can export and import Records.
* **View or Edit Specific Fields in a Table**

  For each Field on all Tables, you can specify whether Users in the Group can view or edit the data in those Fields.

  This can be used where there may be confidential information stored on some Records. For example, you may have a Salary Field on an Employees Table which you would like to be hidden to all Groups except the Management Group.
* **View or Edit Specific Records in a Table**

  You can limit the Records that a User in the Group can view or edit based on the value in a User Field on the Records.

  For example, you may want to only allow Users to edit Projects where they are the assigned Point of Contact. This can be achieved with permissions.

## Configuring Group Permissions for Tables

To configure the permissions for a Group, start by selecting the **Users** tab in the top right hand corner of your Project.

![Permissions Tab](/assets/images/users-tab.jpg "Permissions Tab")

Click **Configure Permissions** next to the Group that you would like to configure permissions for.

![Configure Permissions Button](/assets/images/configure-permissions-button_rs.jpg "Configure Permissions Button")

{% include note.html content="You cannot configure permissions for the default groups: Project Admins, View, Edit." %}

Each [Table](/building-a-project/an-introduction-to-tables) in the Project will be listed. For each Table, you can select the level of access that Users in this Group should have. The access levels are:

1. **Read**

   Users with this permission can view Records in the Table
2. **Create**

   Users with this permission can create new Records in the Table and also get **Read** permissions
3. **Edit**

   Users with this permission can edit existing Records in the Table and also get **Read** and **Create** permissions
4. **Delete**

   Users with this permission can delete existing Records in the Table and also get **Read**, **Create** and **Edit** permissions

To grant Table permissions to a user group, check the checkbox against Read, Create, Edit or Delete for the Table. Note checking a permission level will automatically check other applicable permission e.g. checking **Create** will automatically check **Read**.

For Groups that have been marked as a 'Read-Only' Group, you can only grant Read permissions for Tables for this Group.

![Adding Permissions](/assets/images/adding-permissions_rs.gif "Adding Permissions")

{% include tip.html content="When new Tables are added to a Project, by default no Groups will be granted access except for the default Groups: Projects Admins, View, Edit." %}

To remove table permissions from a user group, uncheck the checkbox against Read, Create, Edit or Delete for the Table.

![Removing Permissions](/assets/images/removing-permissions_rs.gif "Removing Permissions")

{% include tip.html content="Permission changes apply immediately to users." %}

### Configuring Import and Export Permissions

You can restrict whether Groups of Users can use the [import and export](/gridfox-project/import-export) functionality for Tables.

When you are configuring permissions for a Group, to allow Users in the Group to import and export Records in the Table, check the **Can Import / Export** setting.

![Import Export Permissions](/assets/images/import-export-permissions_rs.jpg "Import Export Permissions")

To stop Users from importing and exporting Records in a Table, uncheck the **Can Import / Export** setting for that Table.

### Configuring Field Permissions

To limit which Fields a user can see and edit on Records, configure Restricted Fields for their User Group.

When you are configuring permissions for a Group, to add restrictions on certain Fields in a Table, click the **Manage** button in the **Restricted Fields** column for the Table.

![Field Permissions Button](/assets/images/field-permissions-button_rs.jpg "Field Permissions Button")

Select the field that you would like to restrict from the drop down. It will be added to the Restricted Fields list.

By default this Field will be set to read only for Users in the Group. They will not be able to edit content in this Field but they can still see it. This is indicated by the padlock icon against the field name.

Once you are happy with the restricted fields list, click **Save** in the modal.

![Setting Field Permissions](/assets/images/setting-field-permission_rs.gif "Setting Field Permissions")

To restrict access further and prevent the Users from seeing a Field completely, click the padlock icon after adding the Field to the restricted list. It will change to a struck through eye to indicate that Users in the Group cannot see this Field.

![Setting Field to Hidden](/assets/images/setting-field-to-hidden_rs.gif "Setting Field to Hidden")

To remove the Restricted Fields for the User Group, click **Manage** again. Hover over the field name and click the bin icon. Click **Save** to confirm your changes.

![Removing Restricted Field](/assets/images/removing-restricted-field_rs.gif "Removing Restricted Field")

### Configuring Record Permissions

You can restrict the Records in a Table that a User can view or edit by:

* The value in a user Field matching to the logged in User
* The value in a user Field matching to the logged in User's Group
* The Record was created by the logged in User
* The Record was created by a user in the logged in User's Group

To limit the Records within a Table which a user can see and edit, configure Record Filters for their User Group.

When configuring Group permissions, against the Table that you would like to restrict fields for, click **Manage** in the **Record Filters** column.

![Restricted Records](/assets/images/restricted-records_rs.jpg "Restricted Records")

From the dropdown select a user Field or the 'Created By' option.

By default, this filter will make all Records read only except for those linked to the current user. This is indicated by the lock, to show that they are read only, and the user icon, to show it is for records matching the logged in user only.

You can click the padlock and user icons to change the permission levels as follows:

| Access Level       | Type  | Permissions                                                                                                                                    |
| ------------------ | ----- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Padlock            | User  | The user can edit records where they are set as the user in the specified field. They can view all other records in the table.                 |
| Padlock            | Group | The user can edit records where they are in the same group as the user in the specified field. They can view all other records in the table.   |
| Struck through Eye | User  | The user can edit records where they are set as the user in the specified field. They cannot see any other records in the table.               |
| Struck through Eye | Group | The user can edit records where they are in the same group as the user in the specified field. They cannot see any other records in the table. |

Once you have configured the record permissions for the table, click **Save** on the modal.

![Configuring Record Permissions](/assets/images/configuring-record-permissions_rs.gif "Configuring Record Permissions")

To remove the Record Filters for the User Group, click **Manage** again. Hover over the field name and click the bin icon. Click **Save** to confirm your changes.

![Removing Record Permissions](/assets/images/removing-record-permissions_rs.gif "Removing Record Permissions")