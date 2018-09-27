![](images/Picture-Title.png)

# Lab 200 - Adding Update and Edit Pages to the Web Application

## Introduction

 This lab will walk you through adding pages to your application, adding data and editing data inside the Visual Builder Cloud Service.

## Objectives

- Create Pages to Add and Edit Content
  - Create a page to allow users to add data
  - Create a page to allow users to edit data

## Required Artifacts

- This lab assumes that you have completed the [lab 100](/LabGuide100.md).

## Add Create and Edit Pages

Now that we have a display of our data, the next step is to allow additions and edits to that data. This will allow users to add new wines as they become available and edit the inventory/reserved counts.

### Add Create Page

- In the **Designer View** of our app, click inside the list component but outside an individual item so that the List is selected and the **List View** tag is displayed in blue.

![](images/200/listSelected.png)

- In the right hand menu select the **Quick Start** icon. Then click **Add Create Page**.

![](images/LabGuide200-252f126c.png)

- This will bring up a two step wizard. For the first step, we will click on the **POST /Inventory** and click **Next**.

![](images/LabGuide200-d85827f1.png)

- This will bring us to the **Page Detail** step where we can select the fields we would like to make available for creating new records. We'll select the following:

  - name
  - quantity
  - reserved
  - variant

![](images/LabGuide200-e9c3b310.png)

- Also adjust the **Button Label** to simply "Create" and click **Finish**.

![](images/LabGuide200-1be1d6be.png)

- You will be presented with the main page of the app again. In order to view the new page  select the monitor icon,, and expand **InventoryWebApp --> flows --> main** dropdown then select **CreateInventory**.

![](images/LabGuide200-743dc668.png)

- You should see a view of your new form appear.

![](images/LabGuide200-df2591bd.png)

- With this page created we can toggle to live mode right to interact with the app and add new data. To enable live mode, click the **Live** button above the right side panel.

![](images/200/liveButton.png)

- Once in live mode, enter a new wine and click **Save**. You can enter your favorite wine or use the following example:

  - **name:** ```  Ice  ```
  - **variant:** ```  white  ```
  - **quantity:** ```  50  ```
  - **reserved:** ```  0  ```

![](images/LabGuide200-dc8bd8fe.png)

(The save may take a few seconds, you'll know it's finished when you see the following screen.)

![](images/LabGuide200-b055e910.png)

- To view our new entry click on the tab for your main page.

![](images/LabGuide200-8a1542ea.png)

- Exit Live mode by selecting the Design button.

![](images/LabGuide200-42ac6cc4.png)


- Back in the **main-start** page you'll see our new entry is added to the list, and also note that there is a new **Create** button which was added for us by using the **Quick Start** guide. Buttons are automatically created to link pages inside the quick start guide.

![](images/LabGuide200-b7a2d3dc.png)

### Add Edit Page

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
