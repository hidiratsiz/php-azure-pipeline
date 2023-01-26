 We will test Azure Web App and Azure Pipeline with this Git repository. 
 We will use PHP for coding and write Hello World on the screen.
 I will try to try other codes over time

Create a PHP web app in Azure App Service

In this article
In this article
1. Get the sample repository
2. Deploy your application code to Azure
3. Update and redeploy the app
4. Manage your new Azure app
5. Clean up resources

### Deploy your application code to Azure

1. Sign into the Azure portal.

2. At the top of the portal, type app services in the search box. Under Services, select App Services.
3. On the App Services page, select Create.

4. Fill out the Create Web App page as follows.
   - Resource Group: Create a resource group named myResourceGroup.
   - Name: Type a globally unique name for your web app.
   - Publish: Select Code.
   - Runtime stack: Select PHP 8.0.
   - Operating system: Select Linux.
   - Region: Select an Azure region close to you.
   - App Service Plan: Create an app service plan named myAppServicePlan
5. To change to the Free tier, next to Sku and size, select Change size.

6. In the Spec Picker, select Dev/Test tab, select F1, and select the Apply button at the bottom of the page.
7. Select the Review + create button at the bottom of the page.
8. After validation runs, select the Create button at the bottom of the page. This will create an Azure resource group, app service plan, and app service.
9. After the Azure resources are created, select Go to resource.
10. From the left navigation, select Deployment Center.
11. Under Settings, select a Source. For this quickstart, select GitHub
12. In the section under GitHub, select the following settings:
    - Organization: Select your organization.
    - Repository: php-azure-pipeline
    - Branch: Select the default branch for your repository.
13. Select Save.
14. Once the GitHub integration is saved, from the left navigation of your app, select Overview > URL.
![overview](https://user-images.githubusercontent.com/113396468/214767960-334a9909-04eb-4f8e-8c3a-6ea7f395dcee.png)

The PHP sample code is running in an Azure App Service

Congratulations! You've deployed your first PHP app to App Service using the Azure portal.

![hellowold](https://user-images.githubusercontent.com/113396468/214768048-71b5b129-f202-418b-b92a-91f953baee23.png)
