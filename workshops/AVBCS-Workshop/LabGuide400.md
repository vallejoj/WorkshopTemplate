![](images/Picture-Title.png)  
Updated: July 10, 2018

## Introduction

This lab is one of a series which provides an overview of Oracle Autonomous Visual Builder Cloud Service(VBCS).

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

## Objectives

- Create a mobile page for viewing inventory item details
- Add a REST Service Connection to the application
- Incorporate data retrieved from Service Connection into application

## Required Artifacts

- This lab assumes that you have completed the previous labs in this series and created the items covered in those labs. If you have not, download the `DemoWSApp_MobileLabImport_2.zip` file and after creating an application in VBCS(instructions found in lab 100), import the zip file provided to set up the items created in the previous labs.

# Add a Inventory Details Mobile Page

- Next we'll add a page to display inventory item details and once that is complete we'll incorporate data retrieved from a third party REST endpoint.

- To begin adding the **Details**, open the **main-start** page where we have a list of the inventory items. Open the **Page Structure** panel by clicking the icon that resembles a diagram above the component list. This will make it easy to see all the components and select the **List View** component which we will work with next.

  ![](images/400/pageStructureIcon.png)

- With the **List View** component selected, open the **Quick Start** tab in the right panel and select **Add Detail Page**.

  ![](images/400/addDetailPage.png)

- Select the GET endpoint of the Inventory Business Object and click **Next**.

  ![](images/400/getInventoryEndpoint.png)

- On the **Page Details** step, select the following items in the order listed and then click **Finish**.
  - Name
  - Variant
  - Inventory
  - Reserved

* After selecting the **List View** component from the **Page Structure** list you can close the **Page Structure** panel again by clicking on the icon again to regain screen space.

# Add REST Service Connection

- If you are not already, log in to the Visual Builder Cloud Service(instructions on how to do so are in Lab 100)

- In your application development console, click on **Service Connections** icon in the far left panel. It is the icon that looks like a circle with a line through it and is highlighted blue in the image below.

  ![](images/400/iconServiceConnections.png)

- Click the button **"+ Service Connection"** to create a new service connection instance.

  ![](images/400/addServiceConnection.png)

- In the **Create Service Connection** window, we will choose **Define by Endpoint** as our source.

  ![](images/400/connectionSource.png)

- Leave "GET" the **Method** dropdown menu. Next, enter the following address in the URL field:

  `http://jsonplaceholder.typicode.com/posts/1`

- Select "Retrieve One" in the **Action Hint** dropdown menu, then click **Next**. (For this example we will be doing a simple GET request returning one record)

  ![](images/400/retrieveOne.png)

- You'll see on the next screen that AVBCS populates some fields with information from the address we have provided. The **Service Name** and **Service ID** are filled in for us.

  ![](images/400/serviceName.png)

- Click on the **Test** tab to try our connection and make sure it works. On the **Test** tab, click **Send** and review the data returned.

  ![](images/400/testConnection.png)

- If the data comes back successfully, click **Copy to Response Body** to inform VBCS of the response structure.

  ![](images/400/copyResponse.png)

- Check the **Response** tab to see the response is now in the "Example" text area, then click **Create**.

  ![](images/400/exampleResponse.png)

- Once created, the development console will display the tab of the new service connection.

  ![](images/400/photosConnectionTab.png)

### **STEP 3**: Title of Step 3

- Instructions for Step 3
