---
title: User (Multi-Select) Fields
openGraphImage: ""
---
# User (Multi-Select) Fields

The User (Multi-Select) Field Type can be used for assigning one or many Project Users to a Record.

For example, if you use Gridfox as a project management tool, you could add a Multi-Select User Field to assign Tasks to multiple Users. 

![Multi Select User Example](/assets/images/user-multi-select-static-example.png "Multi Select User Example")

User (Multi-Select) Fields can be specified as a [Required Field](/building-a-project/field-settings#required-fields) for a Table but they cannot be set as a [Unique Field](/building-a-project/field-settings#unique-fields) or a [Reference Field](/building-a-project/reference-fields).

{% include tip.html content="If a Record should only have one assigned value, rather than multiple, use a User Field instead of a User (Multi-Select) Field." %}

## Configuring User (Multi-Select) Field Settings

Once a User (Multi-Select) Field has been [added to a Table](/building-a-project/creating-fields), you can begin configuring some of the settings for this Field. 

Open the Field Settings by clicking on the Field in the [Grid View Editor](/building-a-project/grid-views) or the Explorer.

User (Multi-Select) Fields can be specified as a Required Field or hidden from view in this sidebar. Hidden fields will be displayed in the sidebar beneath the Hidden Fields heading. 

{% include tip.html content="User (Multi-Select) Fields will be given a default Field name when added to a Table, as all other Fields are, e.g. User (Multi-Select) 1, User (Multi-Select) 2 and so forth." %}

![Configuring User (Multi-Select) Field Settings ](/assets/images/multi-select-users-field-settings.gif "Configuring User (Multi-Select) Field Settings ")

## Colour Coding Users

Project Admins can assign colours to Users for the a User (Multi-Select) Field via the [Users](https://deploy-preview-975--gridfox.netlify.app/building-a-project/an-introduction-to-users) tab in the top right of your project. 

![Users tab](/assets/images/users-tab-new.jpg "Users tab")

Here you can amend the Group that Users are in and change their assigned colour. You can also choose to [remove the User](https://gridfox.com/building-a-project/removing-users) from the Project. 

When [updating users](https://gridfox.com/building-a-project/updating-users), all settings that are saved will be then be visualised the User (Multi-Select) Field in your Project. 

![Colour Coding Users ](/assets/images/updating-user-settings-multi-select-fields.gif "Colour Coding Users")

For example, if you wish for a User to be categorised with the colour green, then you will need to configure this setting via the Users tab. If Users are not currently assigned colours in these settings, then this will need to be updated before the User (Multi-Select) Field will show these colours in your Project. 

{% include note.html content="This process is different to working with a List (Multi Select), where all settings are configured in the View Editor. This is because User (Multi-Select) Fields require Users to already have existing access to a project before they can be selected on this Field." %}