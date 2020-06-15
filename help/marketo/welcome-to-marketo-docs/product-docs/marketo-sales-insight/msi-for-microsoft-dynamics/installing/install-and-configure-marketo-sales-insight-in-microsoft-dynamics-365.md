---
unique-page-id: 3571739
description: Install and Configure Marketo Sales Insight in Microsoft Dynamics 365 - Marketo Docs - Product Documentation
title: Install and Configure Marketo Sales Insight in Microsoft Dynamics 365
---

# Install and Configure Marketo Sales Insight in Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Install and Configure Marketo Sales Insight in Microsoft Dynamics 365 - Marketo Docs - Product Documentation

Marketo Sales Insight is a fantastic tool for giving your sales team a "window" into the wealth of data the Marketing team has. Here's how to install and configure.

>[!NOTE]
>
>**Prerequisites**
>
>Complete your [Marketo-Microsoft integration](http://docs.marketo.com/x/E4A2).
>
>[Download the correct solution](http://docs.marketo.com/x/LoJo) for your version of Microsoft Dynamics CRM.

### What's in this article? {#what-s-in-this-article}

[Import Solution](#installandconfiguremarketosalesinsightinmicrosoftdynamics365-importsolution)  
[Connect Marketo and Sales Insight](#installandconfiguremarketosalesinsightinmicrosoftdynamics365-connectmarketoandsalesinsight)  
[Set User Access](#installandconfiguremarketosalesinsightinmicrosoftdynamics365-setuseraccess)

#### Import Solution {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-importsolution}

##### 1. Log in to [Microsoft Office 365](https://login.microsoftonline.com/). {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-logintomicrosoftoffice365.}

![](assets/image2015-3-16-15-58-55.png)

##### 2. Click the ![--](assets/image2015-3-16-16-1-13.png) menu and select CRM. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clickthemenuandselectcrm.}

![](assets/image2015-3-16-16-0-10.png)

##### 3. Click the ![--](assets/image2015-5-13-10-5-8.png) menu. In the drop-down, select Settings, then select Solutions. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clickthemenu.inthedrop-down-selectsettings-thenselectsolutions.}

![](assets/image2015-5-13-10-4-1.png)

>[!NOTE]
>
>**Reminder**
>
>You should already have [installed and configured the Marketo solution](../../../../../welcome-to-marketo-docs/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install-the-marketo-solution-(online).md) before moving forward.

##### 4. Click Import. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clickimport.}

![](assets/image2014-12-12-9-3a5-3a27.png)

1. In the new window, click **Browse**. Choose the [Marketo Sales Insight solution you downloaded in step 1](#InstallandConfigureMarketoSalesInsightinMicrosoftDynamics365-download-msi). Click **Next**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. The solution will upload. You can view the package contents if you like. Click **Next**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Make sure to leave the box **checked** and click **Import**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Feel free to download the log file. Click **Close**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Awesome! You should see the solution now. If it's not there, refresh your screen.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

   ##### Click Publish All Customizations. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clickpublishallcustomizations.}

   ![](assets/image2015-11-10-11-3a15-3a40.png)

#### Connect Marketo and Sales Insight {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-connectmarketoandsalesinsight}

Let's tie your Marketo instance to Sales Insight in Dynamics. Here is how:

>[!NOTE]
>
>**Admin Permissions Required**

1. Log into Marketo and go to the **Admin** section.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Under the **Sales Insight** section, click **Edit API Configuration**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copy the **Marketo Host**, **API URL** and **API User Id** for use in a later step. Enter an **API Secret Key** of your choice and click **SAVE**.

   >[!CAUTION]
   >
   >Don't use an ampersand (&) in your API Secret Key.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >The following fields must be synced with Marketo for *both Lead and Contact* for Sales Insight to work:
   >
   >    
   >    
   >    * Priority 
   >    * Urgency
   >    * Relative Score
   >    
   >    
   >If any of these fields are missing, you will see an error message in Marketo with the name of the missing fields. To fix this, perform [this procedure](../../../../../welcome-to-marketo-docs/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Back in Microsoft Dynamics, click the ![](assets/image2015-5-13-15-3a49-3a19.png)icon next to Settings, then select **Marketo API Config** in the dropdown.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

   ##### Click Default Configuration. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clickdefaultconfiguration.}

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Enter the information that you copied from Marketo earlier.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

   ##### Click the ![](assets/image2015-5-13-16-3a8-3a51.png)icon in the bottom right corner to save the changes. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clicktheiconinthebottomrightcornertosavethechanges.}

#### Set User Access {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-setuseraccess}

You need to give users permissions to use Sales Insight.

##### 1. Click the ![](assets/image2015-5-13-10-3a5-3a8.png)

menu. In the dropdown menu select Settings, then select Security. {#installandconfiguremarketosalesinsightinmicrosoftdynamics365-clickthemenu.inthedropdownmenuselectsettings-thenselectsecurity.}

![](assets/image2015-5-13-16-3a12-3a12.png)

1. Click **Users**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Select the user(s) you want to give access to Sales Insight to and click **Manage Roles**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Select the **Marketo Sales Insight** role and click **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   And you should be all done! Finally, to test, log into Dynamics as a user who has access to Marketo Sales Insight and look at a lead or contact.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

You have now unlocked the power of Marketo Sales Insight for your sales team.

>[!NOTE]
>
>**Related Articles**
>
>[Setting up Stars and Flames for Lead/Contact Records](http://docs.marketo.com/x/BICMAg)
