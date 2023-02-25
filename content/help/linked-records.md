---
seo:
  title: Linked Records | Gridfox
title: Linked Records
---
# Linked Records

In Gridfox, Tables can be linked to one another to create relationships between your Records.

For example, if you were using Gridfox as your custom CRM, a Companies Table could be linked to a Contacts Table. When you are looking at a Contact Record then you could see which Company they work for, and when looking at a Company Record then you could see all the related Contacts which work there.

{% include tip.html content="There are several types of relationships that can be created between Tables. These relationships are created and configured by your Project Admins." %}

When you are viewing a Record, linked Records will display in one of two ways:

1. **As a Field on the Record**

   Here, you can see the related Company when viewing a Contact Record

   ![Company Field on Contact](/assets/images/company-field-on-contact.jpg "Company Field on Contact")
2. **As a list of related Records**

   Here you can see the list of related Contacts when viewing a Company Record

   ![Contact Table on Company](/assets/images/contact-table-on-company.jpg "Contact Table on Company")



When you are [creating](/gridfox-project/creating-records) and [editing](/gridfox-project/updating-records) your Records, you can also change any linked Records.

## Creating Links between Records

When you are looking at a Record which has many related Records from another Table, these related Records will show in a grid below the Record information.

In the example below, the Company Table has a related Opportunity Table and a related Contact Table.

![Linked Records](/assets/images/linked-records.jpg "Linked Records")

When looking at a Company, you can create a new linked Contact by clicking the **Add Record** button and then selecting **New Contact**.

![Add Linked Record Button](/assets/images/add-linked-record-button.jpg "Add Linked Record Button")

If the Contact already exists, you can instead pick the **Existing Contact** option.

Alternatively, when I am looking at a Contact I can create a new linked Company by clicking the **New** button next to the Company Field.

![New Parent Link](/assets/images/new-parent-link.jpg "New Parent Link")

If the Company that you would like to link the Contact to already exists, use the search box to find the Company.