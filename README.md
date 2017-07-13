Beebotte Realtime Connector for Microsoft Azure
===============================================

The Beebotte realtime conector for Azure provides a realtime data connection bridge between Beebotte and Microsoft Azure. It allows to feed data from Beebotte into Azure Event Hubs in real time; Stream Analytics jobs can then be used to process this data in real time for aggregating, correlation, realtime analytics... 

This solution provides an ARM template to directly deploy the package to Azure

### What is included in this package: ###
Markup : * Webjob: A continuous webjob that subscribes to Beebotte channel(s) and publishes data in realtime from Beebotte to Azure Event Hub.
         * Event Hub with its SAS policy: Event Hub is a data streaming platform capable of receiving and processing millions of events per second.
         * US West Basic App Service Plan. 

### How to deploy: ###

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBeebotte%2FBeebotteAzureConnector%2Fmaster%2F%2Fazuredeploy.json"><img src="https://camo.githubusercontent.com/9285dd3998997a0835869065bb15e5d500475034/687474703a2f2f617a7572656465706c6f792e6e65742f6465706c6f79627574746f6e2e706e67" data-canonical-src="http://azuredeploy.net/deploybutton.png" style="max-width:100%;">
	</a>
