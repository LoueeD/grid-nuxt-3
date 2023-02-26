---
seo:
  title: Table Relationship Types | Gridfox
title: Table Relationship Types
---
# Table Relationship Types

There are two relationship types that you can create when [linking Tables](/building-a-project/linking-tables) together in Gridfox: Parent-Child relationship and Many-to-Many relationship.

## Parent-Child relationships

A parent-child relationship, or one-to-many relationship, can be used where you have a single parent Record that will have many child Records.

For example, if you were using Gridfox to track your Projects you may create a parent Project Table and link a child Tasks Table. This will mean one Project can have many Tasks, and each Task is linked to a single Project.

### Using Parent-Child relationships in Gridfox

When you have created a Parent-Child relationship between two Tables, if you look at a Record from the parent Table then there will be a related list of Records from the child Table shown.

For example, if you have created a parent Company Table with a child Contact Table then viewing the Company will show a related list of Contacts.

![Contact on Company](/assets/images/contact-table-on-company.jpg "Contact on Company")

If you were instead looking at the Contact Record, the Company would be shown as a Field since a Contact can only have one linked parent Company.

![Company on Contact](/assets/images/company-field-on-contact.jpg "Company on Contact")

Parent-child relationships can be utilized around your Project in the following ways:

1. **Group Board Columns**

   When configuring a [Board](/building-a-project/board-screens), you can select to group the Records shown by their Parent Record
2. **Group Charts**

   When configuring [Charts](/building-a-project/chart-types) on a Dashboard, for some Chart Types you can select to group the data by the assigned Parent Record
3. **Formula Fields**

   When using a [Formula Field](/building-a-project/formula-fields), you can select to use a Field from a parent Table in your calculation, or to sum based on linked child Records
4. **Group Gantt Charts**

   On a [Gantt Chart](/building-a-project/gantt-screens), you can select to group the Records shown by their Parent Record
5. **ID Masks**

   When setting the [ID Mask](/building-a-project/id-masks) for a Reference Field, you can include Fields from a parent Table to display

If a Table is the child in a parent-child relationship, you can create a relationship with this Table and another Table. For example, you can create a parent Company Table with a child Projects Table. The Projects Table can then be set as the parent Table to a child Tasks table.

When you are [configuring the Screen](/building-a-project/creating-screens#showing-grandchildren-tables-on-screens) for the Company Table, you can select to include the 'grandchild' Tasks Table which will show all Tasks relating to Projects for that Company.

## Many-to-Many relationships

A many-to-many relationship can be used when you have Records between two Tables that will relate to many Records in the other Table.

For example, if you were using Gridfox to track your Customers and which Products they use then you may create a many-to-many relationship between a Customers Table and a Products Table. This means that one Customer can be assigned many Products, and a Product can be utilized by and assigned to many Customers.

### Using Many-to-Many relationships in Gridfox

When you have created a many-to-many relationship between two Tables, if you are looking at a Record in either Table then a related list of Records from the related Table will be shown.

In the example above, where there is a many-to-many relationship between Customers and Products then when you view a Customer the list of related Products will show, and vice versa.

![Product Table on Customer](/assets/images/product-table-on-customer.jpg "Product Table on Customer")

![Customer Table on Product](/assets/images/customer-table-on-product.jpg "Customer Table on Product")

### Many-to-Many relationships and Join Tables

When you select to add a many-to-many relationship between two Tables, you will be given the option of creating a direct relationship or to add a join Table.

Join Tables are useful when you need store some extra information about the relationship between the two related Records.

For example, if you were tracking which of you customers had attended your events then you could create a many-to-many relationship between a Customer Table and an Events Table.

However, you'd probably also want to track whether each customer was invited to the invite and whether or not they attended. A join Table can be used between the Customer Table and Events Table to track attendance.