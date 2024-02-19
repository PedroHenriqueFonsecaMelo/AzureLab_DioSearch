# AzureLab_DioSearch
 
Create an Azure AI Search resource
Sign into the Azure portal.

Click the + Create a resource button, search for Azure AI Search, and create a Azure AI Search resource with the following settings:

Subscription: Your Azure subscription.
Resource group: Select or create a resource group with a unique name.
Service name: A unique name.
Location: Choose any available region.
Pricing tier: Basic
Select Review + create, and after you see the response Validation Success, select Create.

After deployment completes, select Go to resource. On the Azure AI Search overview page, you can add indexes, import data, and search created indexes.

Create an Azure AI services resource
You’ll need to provision an Azure AI services resource that’s in the same location as your Azure AI Search resource. Your search solution will use this resource to enrich the data in the datastore with AI-generated insights.

Return to the home page of the Azure portal. Click the ＋Create a resource button and search for Azure AI services. Select create an Azure AI services plan. You will be taken to a page to create an Azure AI services resource. Configure it with the following settings:
Subscription: Your Azure subscription.
Resource group: The same resource group as your Azure AI Search resource.
Region: The same location as your Azure AI Search resource.
Name: A unique name.
Pricing tier: Standard S0
By checking this box I acknowledge that I have read and understood all the terms below: Selected
Select Review + create. After you see the response Validation Passed, select Create.

Wait for deployment to complete, then view the deployment details.
Create a storage account
Return to the home page of the Azure portal, and then select the + Create a resource button.

Search for storage account, and create a Storage account resource with the following settings:
Subscription: Your Azure subscription.
Resource group: The same resource group as your Azure AI Search and Azure AI services resources.
Storage account name: A unique name.
Location: Choose any available location.
Performance: Standard
Redundancy: Locally redundant storage (LRS)
Click Review and then click Create. Wait for deployment to complete, and then go to the deployed resource.

In the Azure Storage account you created, in the left-hand menu pane, select Configuration (under Settings).
Change the setting for Allow Blob anonymous access to Enabled and then select Save.
Upload Documents to Azure Storage

In the left-hand menu pane, select Containers.
![image](https://github.com/PedroHenriqueFonsecaMelo/AzureLab_DioSearch/assets/83472390/d924db34-7418-43be-9d12-2faf71663761)
Select + Container. A pane on your right-hand side opens.

Enter the following settings, and click Create:
Name: coffee-reviews
Public access level: Container (anonymous read access for containers and blobs)
Advanced: no changes.
In a new browser tab, download the zipped coffee reviews from https://aka.ms/mslearn-coffee-reviews, and extract the files to the reviews folder.

In the Azure portal, select your coffee-reviews container. In the container, select Upload.

![image](https://github.com/PedroHenriqueFonsecaMelo/AzureLab_DioSearch/assets/83472390/6d3fad66-1bca-4028-938a-ec1e78fe19c9)
![image](https://github.com/PedroHenriqueFonsecaMelo/AzureLab_DioSearch/assets/83472390/7666542a-b930-43de-9a9d-0c5dda4d8c32)


In the Containers, select the container coffee-skillset-image-projection. Select any of the items.
Select any of the .jpg files. Select Edit to see the image stored from the document. Notice how all the images from the documents are stored in this manner.
![image](https://github.com/PedroHenriqueFonsecaMelo/AzureLab_DioSearch/assets/83472390/61045527-f418-44a6-a7fe-9b3419c405d6)



