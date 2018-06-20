![](images/100/Picture100-lab.png)  
Updated: February 10, 2017

## Introduction

This is the first of several labs that are part of the **Oracle Autonomous Visual Builder Cloud Service workshop.** This workshop will walk you through creating applications for web and mobile from the browser using a visual development environment.

You will take on 2 Personas during the workshop. The **Javascript Developer Persona** will create the web application and add the associated business data. The Javascript Developer will then create the mobile application and link it to the web applications existing business data. The **IT Security Analyst Persona** will implement access controls in the applications and configure user accounts to allow access to the applications. During the workshop, you will get an overview of Oracle Autonomous Visual Builder Cloud Service and some of its features.

**_To log issues_**, click here to go to the [github oracle](https://github.com/oracle/learning-library/issues/new) repository issue submission form.

## Objectives

- Creating a Web Application
  - Create application within Visual Builder user interface
- Create Application Pages
  - Create pages for business objects
- Add Navigation
  - Add navigation between pages within the application
- Add Pages for Data Manipulation
  - Add pages to allow data insertion, changes, and deletion

## Required Artifacts

- The following lab requires an Oracle Public Cloud account that will be supplied by your instructor.

# Create an Application in Visual Builder Cloud Service

### **STEP 1**: Login to your Oracle Cloud Account

- From any browser, go to the URL:
  `https://cloud.oracle.com`

- click **Sign In** in the upper right hand corner of the browser

  ![](images/100/index.png)

- **IMPORTANT** - Under my services, select from the drop down list the correct data center and click on **My Services**. If you are unsure of the data center you should select, and this is an in-person training event, **_ask your instructor_** which **Region** to select from the drop down list. If you received your account through an Oracle Trial, your Trial confirmation email should provide a URL that will pre-select the region for you.

  ![](images/100/index.png)

- Enter your identity domain and click **Go**.

  **NOTE:** The **Identity Domain, User Name** and **Password** values will be given to you by the instructor or Trial confirmation email.

  ![](images/100/index.png)

- Once your Identity Domain is set, enter your User Name and Password and click **Sign In**

  **NOTE:** For this lab you will assume the role of Javascript Developer **_Lisa Jones_**. Although you are assuming the identify of Lisa Jones, you will log into the account using the **username** provided to you by your instructor, given to you by your corporation, or supplied to you as part of an Oracle Trial. As you progress through the workshop, you will remain logged in as a single user, but you will make “logical” changes from Lisa Jones the Javascript Developer to other personas.

  ![](images/lisa.png)

  ![](images/100/index.png)

- You will be presented with a Dashboard displaying the various cloud services available to this account.

  ![](images/100/index.png)

- If all your services are not visible, **click** on the **Customize Dashboard**, you can add services to the dashboard by clicking **Show.** For this workshop, you will want to ensure that you are showing at least the **Application Container, Developer and Storage** cloud services. If you do not want to see a specific service, click **Hide**

  ![](images/100/index.png)

### **STEP 2**: Access the Oracle Autonomous Visual Builder Cloud Service

Oracle Autonomous Visual Builder Cloud Service provides an easy way to
create and host web and mobile applications in a secure cloud
environment. An intuitive visual development experience on top of a
complete development and hosting platform accelerates application
creation and provisioning, leveraging an open, standard-based
architecture.

- From the Cloud UI dashboard click on the **Visual Builder** service.

  ![](images/100/index.png)

- The Service Details page gives you a quick glance of the service status overview.

  ![](images/100/index.png)

- Click **Open Service Console** for the Oracle Visual Builder Cloud Service. The Service Console will then list all Visual Applications.

  ![](images/100/index.png)

### **STEP 4**: Create Visual Application

- Click **New** to start the application create wizard.

  ![](images/100/vbcsca_cra_s2.png)

- On Details screen enter the following data and click on **Next**.

  In the Create Application dialog box, enter the following.

  - Application name: Application
  - Description: Tutorial application

  - The Application ID text field is automatically populated as you type based on the Application Name.
    ![](images/100/index.png)

- The Project Creation will take a few minutes.

  ![](images/100/index.png)

- You now have a new application, in which you can begin building pages and adding data.

  ![](images/100/index.png)

## Import Business Data

### **STEP 5**: Import File containing business data

In this step you are still assuming the identity of the Javascript, **_Lisa Jones_**.

![](images/lisa.png)

- Click **Issues** on left hand navigation panel to display the Track Issues page.

  ![](images/100/Picture100-16.png)

- Click **New Issue**. Enter the following data in the New Issue page and click **Create Issue**.

  **Note:** Throughout the lab you will assign your own account as the “physical” owner of the issue, but for the sake of this workshop, **Bala Gupta** will be the “logical” owner of the following issues.

  ![](images/bala.png)

  **Summary:**
  `Create Initial GIT Repository for Twitter Feed Service`

  **Description:**
  `Create Initial GIT Repository for Twitter Feed Service`

  **Type:** `Task`

  **Owner:** `Select your account provided in the dropdown [Logical Owner: Bala Gupta]`

  **Story Points:** `1`

  Note: Story point is an arbitrary measure used by Scrum teams. They are used to measure the effort required to implement a story. This [Site](https://agilefaq.wordpress.com/2007/11/13/what-is-a-story-point/) will provide more information.

  ![](images/100/Picture100-17.png)

### **STEP 6**: Create Issue for Update Twitter Credentials

- Click **New Issue**. Enter the following data in the New Issue page and click **Create Issue**.

  ![](images/bala.png)

  **Summary:** `Create Filter on Twitter Feed`

  **Description:** `Create Filter to allow user to supply text to reduce the amount of data returned by the Twitter feed`

  **Type:** `Feature`

  **Owner:** `Select your account provided in the dropdown [Logical Owner: Bala Gupta]`

  **Story Points:** `2`

  ![](images/100/Picture100-18.png)

### **STEP 7**: Create Issue for initial GIT Repository creation

- Click **New Issue**. Enter the following data in the New Issue page and click **Create Issue**. Note: The next two issues will logically be owned by John Dunbar.

  ![](images/john.png)

  **Summary:** `Create Initial GIT Repository for Twitter Feed Marketing UI`

  **Description:** `Create Initial GIT Repository for Twitter Feed Marketing UI`

  **Type:** `Task`

  **Owner:** `Select your account provided in the dropdown [Logical Owner: John Dunbar]`

  **Story Points:** `1`

  ![](images/100/Picture100-19.png)

### **STEP 8**: Create Issue for Displaying Twitter Feed

- Click **New Issue**. Enter the following data in the New Issue page and click **Create Issue**.

  ![](images/john.png)

  **Summary:** `Display Twitter Feed in Table Format`

  **Description:** `Display Twitter Feed in Table Format`

  **Type:** `Feature`

  **Owner:** `Select account provided in the dropdown [Logical Owner: John Dunbar]`

  **Story Points:** `2`

  ![](images/100/Picture100-20.png)

- Click the back arrow ![](images/100/Picture100-21.png) on the **left side** of the window, or click on the **Issues** menu option to view all newly created issues.

  ![](images/100/Picture100-22.png)
