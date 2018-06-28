![](images/Picture-Title.png)  
Updated: June 27, 2018

## Introduction

This is the second of several labs that are part of the **Oracle Autonomous Visual Builder Cloud Service workshop.** This workshop will walk you through creating applications for web and mobile from the browser using a visual development environment.

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

## Objectives

- Create Pages to Add and Edit Content
  - Create a page to add data
  - Create a page to edit data

## Required Artifacts

- The following lab requires an Oracle Public Cloud account that will be supplied by your instructor.

# Add Create and Edit Pages

Now that we have a display of our data, the next step is to allow additions and edits to that data. This will allow users to add new wines as they become available and edit the inventory/reserved counts. Oracle Autonomous Visual Builder makes this very easy with the **Quick Start** menu we accessed earlier.

- In the **Designer View** of our app, click inside the list component but outside an individual item so that the List is selected and the **List View** tag is displayed.

![](images/200/listSelected.png)

- This will allow you to access the **Quick Start** icon and menu where we'll select **Add Create Page**.

![](images/200/addCreatePage.png)

- This will bring up the **Add Create Page**. For the first step, we will leave the endpoint set as **POST /Inventory** and click **Next**. This will bring us to the **Page Detail** step where we can select the fields we would like to make available for creating new records. We'll select the following:

  - name
  - variant
  - inventory
  - reserved

- Also adjust the **Button Label** to simply "Create" and click **Finish**.

  ![](images/200/createInventoryDetail.png)

- You will be presented with the main page of the app again. In order to view the new Create Page click the icon to expand the left panel, select the monitor icon which represents web apps, and if you have not expanded the app's layout expand **InventoryWebApp** > **flows** > **main** and select **CreateInventory**.

  ![](images/200/createPageView.png)

With this page created we can toggle live mode right in the app editor to interact with the app and add data. To enable live mode, click the **Live** button above the right side panel.

![](images/200/liveButton.png)

- Once in live mode, enter a new wine and click **Save**.(The save may take a few seconds, you'll know it's finished when you see the following screen and a notification that the save completed) You can enter your favorite wine or use the following example:

  - name: Ice
  - variant: white
  - quantity: 50
  - reserved: 0

  ![](images/200/newWine.png)

  ![](images/200/flow.png)

- To view our new entry let's go back to our apps main page, which you can access in the left side panel or in the tabs at the top of the page if you have not closed it. (Don't forget to exit live mode when you go back to the **CreateInventory** page designer by clicking on the "Play" arrow button.)

  ![](images/200/pageTabs.png)

- Back in the **main-start** page you'll see our new entry is added to the list, and also note that there is a new **Create** button which was added for us by using the **Quick Start** guide to make our new create page. This is a major advantage to using the quick start guide for creating new pages, it will make buttons for us that will link to our new pages.

- Now lets use the **Quick Start** guide to add an **Edit** page and a **Delete** button to our app's main page. Once again, click on the **List** component outside of a specific item so that the **List View** tag appears.

  ![](images/200/listSelected.png)

- Now the **List View** detail panel should be displayed on the right. Click on the **Quick Start** icon and we'll see the links to add pages. This time we'll add an **Edit** page. This will allow users to edit the inventory and reserve counts of the items. Click on **Add Edit Page** in the right panel.

  - ![](images/200/addEditPage.png)

- On the **Select Read Endpoint** page we'll leave the default endpoint selected (GET /Inventory/{Inventory_Id}), and click **Next**. On the next step we'll leave the **Select Update Endpoint** set as the default (PATCH /Inventory/{Inventory_Id}) and click **Next**.

- In the **Page Details** step we'll select the fields we want displayed on our edit page, and then click **Finish**. Here we'll select:

  - Name
  - Variant
  - Quantity
  - Reserved

  ![](images/200/editFields.png)

- Now if we go back to our "Main-start" page and again enter **Live** mode by clicking the "Live" button above the right panel we can test our edit page. Click on a list entry and the the **Edit Inventory** button will become active. Click on the **Edit Inventory** button to go to our new edit page we just created.

  ![](images/200/editLive.png)

- This section of the web app will allow users to update items with new counts as they become available. If you would like to test the edit functionality, change a count and press save, otherwise just press cancel to return to the **main-start** page. Remember to exit **Live** mode by clicking the "Live" button in the top right.

- If we go back to our **main** tab we can now see our apps structure:

![](images/200/structure.png)

# Summary

We have now created an application in Autonomous Visual Builder Cloud Service, added our business data, and added pages to display, add to, and edit our data all with very little need for code.
