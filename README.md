Beebotte Realtime Connector for Microsoft Azure
===============================================

The Beebotte realtime conector for Azure provides a realtime data connection bridge between Beebotte and Microsoft Azure. It allows to feed data from Beebotte into Azure Event Hubs in real time; Stream Analytics jobs can then be used to process this data in real time for aggregating, correlation, realtime analytics... 

This solution provides an ARM template to directly deploy the package to Azure

### What is included in this package: ###
* Webjob: A continuous webjob that subscribes to Beebotte channel(s) and publishes data in realtime from Beebotte to Azure Event Hub.
* Event Hub with its SAS policy: Event Hub is a data streaming platform capable of receiving and processing millions of events per second.
* US West Basic App Service Plan. 

### How to deploy: ###

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBeebotte%2FBeebotteAzureConnector%2Fmaster%2F%2Fazuredeploy.json"><img src="https://camo.githubusercontent.com/9285dd3998997a0835869065bb15e5d500475034/687474703a2f2f617a7572656465706c6f792e6e65742f6465706c6f79627574746f6e2e706e67" data-canonical-src="http://azuredeploy.net/deploybutton.png" style="max-width:100%;">
	</a>
	<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FBeebotte%2FBeebotteAzureConnector%2Fmaster%2F%2Fazuredeploy.json"><img src="https://camo.githubusercontent.com/536ab4f9bc823c2e0ce72fb610aafda57d8c6c12/687474703a2f2f61726d76697a2e696f2f76697375616c697a65627574746f6e2e706e67" style="max-width:100%;">
	</a>

1. Click on the “Deploy to Azure” button above.
2. This will redirect you to the Azure portal login page if you are not already logged in to Azure.
3. After login, the ARM template will appear.

Follow the steps below to deploy the ARM template to your Azure subscription:

1. Select your Azure Subscription that you want to associate this deployment with.
2. Create a new, or use an existing Resource Group to deploy all the components of this template to.
3. For Location, select West US. 
4. For the Event Hub Namespace, enter a unique Namespace.
5. For the Azure Web Job Name, create a unique Web Job Name.
6. For the Beebotte Channel, enter a channel name that the connector should subscribe to. You can enter a comma delimited list of channels in the following format: channel1.*,channel2.resource2,channel3. Use channel.* or simply channel to subscribe to all the resources of a channel; use channel.resource if you want to subscribe to a specific resource within a channel.
7. For the Beebotte API Key, enter the API key of your Beebotte account.
8. For the Beebotte Secret Key, enter the API Secret Key of your Beebotte account.
9. For the Azure Service Plan, enter USWestBasic.
10. For the Azure SAS Policy Name, enter a unique name.
11. Check the I agree to the terms and conditions stated above checkbox.
12. Click Purchase.

### Support: ###
For any issue or concern, contact support@beebotte.com

