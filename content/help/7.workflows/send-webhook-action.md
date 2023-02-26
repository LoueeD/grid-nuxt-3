---
seo:
  title: Send Webhook Action | Gridfox
title: Send Webhook Action
---
# Send Webhook Action

Using the 'Send Webhook' Workflow Action, you can post data from your Gridfox Records to arbitrary endpoints.

{% include note.html content="The 'Send Webhook' action can only be used in Workflows that are triggered by the create or update of a Record." %}

## Adding a Send Webhook Action

Start by opening up the Workflow that you would like to add a 'Send Webhook' action to, or [create a new Workflow](/building-a-project/creating-workflows).

Drag the 'Send Webhook' block onto the canvas and click the block to open the configuration panel.

![Add Send Webhook Workflow Action](/assets/images/add-send-webhook-action_rs.gif "Add Send Webhook Workflow Action")

### Specifying Webhook URL

Firstly, enter the endpoint URL in the 'Webhook' URL field.

![Webhook URL Field](/assets/images/webhook-url_rs.jpg "Webhook URL Field")

### Specifying Authentication Method

If required, choose an authentication method for your request in the 'Webhook Authentication Type' menu.

#### API Key

When using an API key, you must enter the Header name and the API key value.

### OAuth

Gridfox supports the Client Credentials grant type for OAuth 2.0. Enter the token endpoint, client ID, client secret and optionally the scope.

### Specifying Payload

Finally, specify the payload that should be sent.

Add the payload details by clicking the plus icon in the 'Webhook Body' section. You can then add in the key and value information as required.

To include information from the record that triggered the workflow, you can enclose the field name in square brackets when defining the webhook body.

{% include tip.html content="Only Fields from the Record itself can be included, rather than Fields from any related Records." %}