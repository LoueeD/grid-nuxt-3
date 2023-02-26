---
seo:
  title: "Creating Forms | Gridfox "
title: Creating Forms
---
# Creating Forms

Forms can be used to capture information from anyone, directly creating Records in your Gridfox Project.

{% include tip.html content="You can create multiple Forms for the same Table." %}

## Creating a new Form

1. Select the **Forms** tab in the top right hand corner
2. Click **New Form**
3. Enter a Form Name
4. Choose which [Table](/building-a-project/an-introduction-to-tables) you would like the Form to create Records for

   All the [Fields](/building-a-project/an-introduction-to-fields) currently available on the selected Table will now be shown on the Form
5. Enter a title for the Form and optionally a description

   These will be shown to the people that view your Form
6. Click **Save & Share**

![Creating a new Form](/assets/images/creating-a-new-form.gif "Creating a new Form")

## Configuring Form Fields

By default, all supported Fields currently on the Table will be shown on the Form.

Fields of Type User, Auto Counter and Formula cannot be shown on Forms. You also cannot include linked Fields such as parent link Fields or Many-to-many link Fields.

To hide a Field, drag and drop it into the hidden Fields section on the left. You can also click the **Hide Field** button for the Field.

![Hiding Form Fields](/assets/images/hiding-form-fields_rs.gif "Hiding Form Fields")

To show a Field again, either drag it back onto the Form or click the plus button to the right of the Field name.

![Showing Form Fields](/assets/images/showing-form-fields_rs.gif "Showing Form Fields")

{% include tip.html content="If you [add a new Field](/building-a-project/creating-fields) to a Table, it will not be shown by default on any existing Forms for that Table." %}

To reorder the Fields on your Form, drag them up and down the list. Alternatively you can use the up and down arrows within a Field.

![Reordering Form Fields](/assets/images/reordering-form-fields_rs.gif "Reordering Form Fields")

By default, all Fields will have be labelled with the Field name of the Field they relate to. You can change the Field label by clicking into the Field and changing the label text.

![Renaming Form Fields](/assets/images/renaming-form-fields_rs.gif "Renaming Form Fields")

## Setting Form Fields as Required

To ensure people give you all the data you need, you can make Form Fields required for submission. Note that this makes the Field required on the Form only, not on the Table itself.

Fields that have been [set to be required](/building-a-project/field-settings#required-fields) on the Table cannot be made optional on the Form.

1. Click on the Field that you want to set as required
2. Toggle the **Required** setting to on
3. Click **Save & Share**

If you no longer want the Field to be marked as required, simply change toggle this setting off.

![Setting Fields as Required](/assets/images/required-form-fields_rs.gif "Setting Fields as Required")

## Specifying Default Values for Form Fields

You can choose to set default values in Form Fields. When someone fills in your Form, default values will be shown.

1. Click on the Field that you want to set the default value for
2. Click the settings cog for that Field
3. Enter or choose a default value
4. Click **Save & Share**

![Default Form Value](/assets/images/set-default-form-value_rs.gif "Default Form Value")

## Setting Form Colour Scheme

You can choose the colour to use for the Form banner.

1. Click **Set Colour** in the top right
2. Choose a pre-set Form colour option

   Alternatively set your own custom colour by clicking the paint can icon
3. Click **Save & Share** to finalise your change

![Setting Form Colour](/assets/images/setting-form-colour_rs.gif "Setting Form Colour")

## Customising the Form Submission message

You can optionally add a custom message that shows when someone submits a Form response. This could be used to confirm response times to an enquiry, to add a link to your FAQs or website, or to thank them for their response.

{% include note.html content="If you do not specify a Submission Message, then the default Form submission page will be shown." %}

To specify a Submission Message, either scroll to the bottom of the Form or click the **Settings Cog** in the Form Settings panel.

![Form Settings Button](/assets/images/form-settings-button.jpg "Form Settings Button")

Enter in the message that you would like to show to people that submit a response to this Form.

{% include tip.html content="There is a character limit of 1000 characters on this message." %}

![Form submission message](/assets/images/form-submission-message_rs.gif "Form submission message")

## Previewing a Form

To take a look at your Form before you share it, click the **Preview** button.

![Preview Form Button](/assets/images/preview-form-button_rs.jpg "Preview Form Button")

From the preview you can adjust the colour scheme and also choose to save or share the Form.

To return to the Form configuration screen, click **Exit Preview** or **Back to Editor**.

## Sharing a Form

To share your Form, hover over the **Save & Share** button and copy the URL.

Anyone with this link can now submit a Form response.

{% include note.html content="The Form link will remain fixed, even if you change the Form configuration. If you make changes to a Form that has been shared, remember that these changes will show as soon as you save the changes to the Form." %}

When a Form response is submitted, Records will be created in the appropriate Table in your Project. In the [Record History](/gridfox-project/record-history), the Record will show to have been created by a Form submission. Any [Workflows](/building-a-project/an-introduction-to-workflows) that are set to trigger on Records creation will be triggered.