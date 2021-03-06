page_main_title: Key-value
main_section: Reference
sub_section: Integrations
page_title: Key-value integration

# Key-value pair integration

A key-value pair integration is a custom integration where you can give any key-value pairs. You can use it in your ci or pipeline jobs. These key-values will be available as environments variables to you.

##Adding your Key-Value Pair integration

-  Go to your **Account Settings** by clicking on the gear icon in the top navigation bar.

<img src="../../images/reference/integrations/account-settings.png" alt="Add key-values">

-  Click on **Integrations** in the left sidebar menu and then click on **Add integration**
-  Locate **Key-Value pair** in the list and click on **Create Integration**
-  Name your integration and enter your key-value pairs
-  Choose the Subscription which contains the repository for which you want to use this integration
-  Click **Save**

<img src="../../images/reference/integrations/key-value-integration.png" alt="Add Key-Value pair credentials">

##Editing your Key-Value pair integration

You can go to your **Account Settings** at any time, click on **Integrations** in the left sidebar menu, and click the **Edit** button for your Key-Value pair integration. You can then change integration name,  update keys or values and add or delete key-value pairs.

However, you cannot edit the list of Subscriptions that are allowed to use the integration from this page. To add your integration to additional Subscriptions, read our Adding your integration to additional Subscriptions section

##Deleting your Key-Value pair integration

If you no longer need the integration, you can delete it by following the steps below. Please note that if any projects are using this integration in their `yml` files, builds will fail after deleting the integration:

-  Go to your **Account Settings** by clicking on the gear icon in the top navigation bar.

<img src="../../images/reference/integrations/account-settings.png" alt="Account settings">

-  Click on **Integrations** in the left sidebar menu.
- Locate the integration you want to delete and click on the **Delete** button.
- If there are no Subscriptions using this integration, you will be able to delete it by clicking on **Yes**. You are done at this point.

<img src="../../images/reference/integrations/confirm-delete-integration.png" alt="Delete integration confirmation screen">

- If your integration is being used by any Subscriptions, you will see a message telling you which Subscriptions are still using the integration.

<img src="../../images/reference/integrations/cannot-delete-integration.png" alt="Cannot delete integration because of dependencies">

- Go to each Subscription listed in the dependencies and delete it from each.
    - From the Subsciption dropdown menu at the top left of your Dashboard, click on the dependent Subscription.

    <img src="../../images/reference/integrations/list-subscriptions.png" alt="List subscriptions">

    - Go to the **Settings** tab and click on **Integrations** in the left sidebar.
    - Delete the integration.
- Once you have delete the integration from all Subscriptions, you can go back to **Account Settings** and delete the integration.
