---
seo:
  title: Multifactor Authentication | Gridfox
title: Multifactor Authentication
---

# Multifactor Authentication

To add some extra security to your Gridfox Account, you can enable Multifactor Authentication on your user login. When you login, you will be prompted to enter a code from an authenticator app.

{% include tip.html content="Multifactor Authentication can be enabled at an Account level also which will mean anyone who accesses Projects in your Account will have to use multifactor authentication. See the [Account Admin help](/building-a-project/enabling-multifactor-authentication) for more details." %}

## Enabling Multifactor Authentication for your Login

To set this up, open up the Account Management Section by clicking the **Account Menu** in the top right hand corner and select **Settings**.

![Account Menu Settings](/assets/images/account-menu-settings.jpg 'Account Menu Settings')

Click the **Manage** button in the Multifactor Authentication section within your Profile.

![Manage MFA Button](/assets/images/manage-mfa.jpg 'Manage MFA Button')

Click **Enable** on the following page.

![Enable MFA Button](/assets/images/enable-mfa-button.jpg 'Enable MFA Button')

You will then be presented with a QR code that you can scan using your preferred authenticator app. Then enter in the code you receive from your authenticator app and click **Enable**.

![MFA QR Code](/assets/images/mfa-qr-code.jpg 'MFA QR Code')

If the code is entered correctly, Multifactor Authentication will be enabled for your user login. You will need to use the authentication each time you log into Gridfox.

{% include tip.html content="Remember to save the recovery codes just in case you lose access to the authenticator device." %}

## Disabling Multifactor Authentication for your Login

You can choose to disable Multifactor Authentication for your user login at any time. Select the **Account Menu** in the top right hand corner of the screen and choose **Settings**.

![Account Menu Settings](/assets/images/account-menu-settings.jpg 'Account Menu Settings')

Click the **Manage** button in the Multifactor Authentication section within your Profile.

![Manage MFA to Disable](/assets/images/manage-mfa-to-disable.jpg 'Manage MFA to Disable')

Click **Disable** on the following page.

![Disable MFA](/assets/images/disable-mfa.jpg 'Disable MFA')

Enter the code from your authenticator app to confirm the action and click **Disable**.

![Confirm disable MFA](/assets/images/disable-mfa-confirm.jpg 'Confirm disable MFA')

If the code is entered correctly, Multifactor Authentication will be disabled for your user login.

{% include note.html content="If Multifactor Authentication has been enabled on other Accounts that you have been invited to Projects for, you will still need to use Multifactor Authentication to access these Projects." %}
