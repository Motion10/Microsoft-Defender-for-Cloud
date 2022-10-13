# Module 14 – Configuring Azure ADO Connector in Defender for DevOps

<p align="left"><img src="../Images/asc-labs-intermediate.gif?raw=true"></p>

#### 🎓 Level: 200 (Intermediate)
#### ⌛ Estimated time to complete this lab: 30 minutes

## Objectives
In this exercise, you will learn how to configure Azure ADO Connector in Defender for DevOps.

### Exercise 1: Preparing the Environment

If you alredy finished [Module 1](https://github.com/Azure/Microsoft-Defender-for-Cloud/blob/main/Labs/Modules/Module-1-Preparing-the-Environment.md) of this lab, you can skip this exercise, otherwise plesae finish at least Exercise 1, 2 and 3 from Module 1.

### Exercise 2: Creating an Azure ADO Trial Subscription

1.	Open an In-Private session in your web browser and navigate to [https://dev.azure.com](https://dev.azure.com)
2.	On the main part of this page, click Start free and use your Microsoft account credentials to login. If you don’t want to use your existing credentials, use the Azure Trial subscription account in order to login.
3.	Type your Account email address and Password and login to your DevOps environment..

### Exercise 3: Configuring Azure ADO Connector

1.	Login to your Azure Portal and open Defender for Cloud dashboard
2.	In the left navigation pane, click **Environment settings** option
3.	Click the **Add environment** button and click **Azure DevOps (preview)** option. The **Create Azure DevOps connection** page appears as shown the sample below.

![Azure ADO Connector](../Images/M14_Fig1.PNG?raw=true)

4.	Type the name for the connector, select the subscription, select the Resource Group, which can be the same you used in this lab and the region. 
11.	Click **Next:select plans >** button to continue.
12.	In the next page leave the default selection with **DevOps** selected and click **Next: Authorize connection >** button to continue. The following page appears:

![Azure ADO Connector - Authorize](../Images/M14_Fig2.PNG?raw=true)


13.	Click **Authorize** button. If this is the first time you’re authorizing your DevOps connection, you’ll receive a pop-up screen, that will ask your permission to authorize. Scroll down the popped up window screen and click the **Accept** button as shown in the sample below:

![Azure ADO Connector - Accept](../Images/M14_Fig3.PNG?raw=true)

> **Note** When you click **Accept** in your Azure DevOps, you’ll notice the proof of Authorization to the **Microsoft Security DevOps** App. You can find this in your Azure ADO organization, under the **Personal Access tokens** / **User Settings** / **Authorizatons**.  

14.	After the authorization is complete, you will need to select your Azure ADO organization and projects as shown in the sample below:

![Azure ADO Connector - Accept](../Images/M14_Fig4.PNG?raw=true)

15.	After selecting the organization, keep the option **Auto discovery of projects** enabled.
16.	Click **Review and create** button to continue.

> **Note** You need to be a **Project Collection Admin** in the Azure DevOps organization that you selected to complete this process. Learn more about this role [here](https://learn.microsoft.com/en-us/azure/devops/organizations/settings/about-settings?view=azure-devops&WT.mc_id=Portal-Microsoft_Azure_Security_DevOps#project-collection-administrator-pca-role-and-managing-collections-of-projects)

17.	After some minutes you will see the Azure DevOps connector in the **Environment settings** page and in about 15 minutes, you will start to seeing the total resources number populating.



### Continue with the next lab: [Module 15 – Configuring GitHub Connector in Defender for DevOps](Module-8-Advance-Cloud-Defense.md)