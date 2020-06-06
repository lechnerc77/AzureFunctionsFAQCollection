# AzureFunctionsFAQCollection
This is just a simple collection of FAQs on Azure Functions that I stumbled across and I wanted to memorize somewhere I could access them ... from any place :-)
No warranty that the stuff is correct

## General Ressources for tips and tricks
[Azure Tips and Tricks](https://microsoft.github.io/AzureTipsAndTricks/)

## Custom Handlers
Bring your own language by implementing [custom handlers](https://docs.microsoft.com/en-US/azure/azure-functions/functions-custom-handlers)

## Custom Bindings
You can create your own bindings and use them in Azure Functions. Here is how this can be achieved [link](https://microsoft.github.io/AzureTipsAndTricks/blog/tip247.html).

## Canary Deployment
In general, there are different types of deployment. An overview is given in this [article](https://azure.microsoft.com/de-de/blog/deployment-strategies-defined/).

A canary deployment is possible with Azure Functions. However, you must run your function under an *App Service Plan* in order to be able to use multiple slots, necessary for this deployment type. You find an overview about deployment slots [here](https://docs.microsoft.com/en-US/azure/azure-functions/functions-deployment-slots).
Another option might be using [API management](https://docs.microsoft.com/en-us/azure/api-management/) or [Azure Traffic Manager](https://docs.microsoft.com/en-us/azure/traffic-manager/traffic-manager-routing-methods#weighted) for routing.

## Scaling of Azure Durable Functions
While the scaling of stateless Azure FUnctions is basically infinite there are some points that need to be considered when using Azure Durable Functions and Azure Durable Entities. The blog post [How Azure Durable Functions scale](https://zure.com/en/blog/how-azure-durable-functions-scale/) gives some valuable insight.
