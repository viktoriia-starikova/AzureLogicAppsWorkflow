# AzureLogicAppsWorkflow
- Azure Logic Apps Workflow
    - Reads events from Azure Service Bus Topics - one at a time
    - Checks that the image does not exceed N MB (this parameter is set in App Logic)
    - If not exceeded, causes image processing (see 3)
    - If it exceeds, which changes the state in Azure Cosmos DB of the task to error
