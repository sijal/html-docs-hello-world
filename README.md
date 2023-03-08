---
topic: HTML Hello World
languages:
  - HTML
products:
  - Azure App Service
  - Azure Web Apps
---

# HTML Hello World

This sample demonstrates a tiny Hello World HTML app for [App Service](https://docs.microsoft.com/azure/app-service).

# Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


# Open Azure Cloud Shell and execute following commands
> mkdir htmlapp
> git clone https://github.com/Azure-Samples/html-docs-hello-world.git
> resourceGroup=$(az group list --query "[].{id:name}" -o tsv)
appName=az204app$RANDOM
> cd html-docs-hello-world
> az webapp up -g $resourceGroup -n $appName --html
> code index.html
> az webapp up -g $resourceGroup -n $appName --html 
