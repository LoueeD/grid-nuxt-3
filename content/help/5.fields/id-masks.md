---
seo:
  title: ID Masks | Gridfox
title: ID Masks
---
# ID Masks

ID Masks can be used on Reference Fields to help display useful information to your Users when they are looking at related Records.

Once you have selected a [Reference Field](/building-a-project/reference-fields) for a Table, this is the information that will show when a User is searching for a Parent Record to [link](/building-a-project/linking-tables) a Child Record to.

For example, you can create a Company Table which has a Reference Field called Company ID that is an Auto Counter. When you create a Company Record, it will be given a unique number in the Company ID Field.

![Company Table with ID Field](/assets/images/company-id-field.jpg "Company Table with ID Field")

You can create a Contacts Table and link it to the Companies Table, so that a Company can have many associated Contacts. For more information on how to create relationships between Tables, see the [Linking Tables](/building-a-project/linking-tables) help.

![Companies with Contacts](/assets/images/companies-with-contacts.jpg "Companies with Contacts")

When you are creating a Contact Record, since the Reference Field for Company is an Auto Counter, the list of Companies to assign the Contacts to will show as a list of numbers.

![Creating a Contact](/assets/images/creating-contact.jpg "Creating a Contact")

To help improve the experience for your Users, you can set an ID Mask on the Reference Field which will result in additional Record information being shown in this dropdown.

For instance, you could include the Company Name in the ID Mask and so the dropdown would show: Axil (1), PIO (2), Overleap (3). The User then knows exactly which Company to select.

ID Masks will show in the following places:

* If you have grouped a Chart by Parent, the ID Mask of the Parent will show as the Chart label
* If you have grouped a Board by Parent, the row or column name will display the ID Mask
* In the Parent field when creating or editing a Child Record, the ID Mask will display in the Field
* When filtering Child Records on a Parent Field, the ID Mask will display in the filter

## Specifying ID Masks on Reference Fields

ID Masks can be specified in either the Grid View Editor or the Explorer.

Click on a Reference Field to open the left hand configuration panel. A section will show for specifying the ID Mask 

![ID Mask Formula](/assets/images/id-mask_rs.jpg "ID Mask Formula")

You can then enter the required ID Mask formula.

To show the value from a Field in an ID Mask, include the Field Name in square brackets. You can include static text also.

For example, if you wanted to include the name of the company in the ID Mask, include `[Name]` in the ID Mask. If you also wanted to include the industry that the company is in, add `[Industry]` to the ID Mask.

You must include the Reference Field itself within the ID Mask. In the above example this would be `[Company ID]`.

You can include Fields from Parent Tables within an ID Mask. To do this, include the Table Name then enter a dot before the Field name. For example, if you wanted to specify an ID Mask for the Contact Reference Field, you could include the name of the Company of the Contact in the ID Mask by using `[Company.Name]`.

You can also include plain text within the ID Mask. This may be useful for adding brackets or dashes between pieces of information.

Enter the ID Mask then click **Validate ID Mask**. This will check if the ID Mask has been defined correctly.

{% include tip.html content="The ID Mask is case sensitive. Make sure to match the Field Name exactly." %}