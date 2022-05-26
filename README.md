# Azure Function Automate Task
local Functions project

https://docs.microsoft.com/en-us/azure/azure-functions/functions-run-local?tabs=v4%2Cwindows%2Ccsharp%2Cportal%2Cbash#install-the-azure-functions-core-tools

Developing functions on your local computer and publishing them to Azure using Core Tools follows these steps:

- Install the Core Tools and dependencies.
- Create a function app project from a language-specific template.
- Register trigger and binding extensions.
- Define Storage and other connections.
- Create a function from a trigger and language-specific template.
- Run the function locally.
- Publish the project to Azure.

Prerequisites

The specific prerequisites for Core Tools depend on the features you plan to use:

Publish: Core Tools currently depends on either the Azure CLI or Azure PowerShell for authenticating with your Azure account. This means that you must install one of these tools to be able to publish to Azure from Azure Functions Core Tools.

Install extensions: To manually install extensions by using Core Tools, you must have the .NET Core 3.1 SDK installed. The .NET Core SDK is used by Core Tools to install extensions from NuGet. You don't need to know .NET to use Azure Functions extensions.

Changing Core Tools versions

When changing to a different version of Core Tools, you should use the same package manager as the original installation to move to a different package version. For example, if you installed Core Tools version 2.x using npm, you should use the following command to upgrade to version 3.x:

npm install -g azure-functions-core-tools@3 --unsafe-perm true
