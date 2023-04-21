# theweatherfool
azuretestTNE
#Steps on how to get Deploy Web App to Azure

Azure CLI Run - az group list
Get the sub id for the resource group #
Example:
{
    "id": "/subscriptions/f2dbdda2-ad28-4b56-998d-d2c9d4046bab/resourceGroups/apim-demo-devops",
    "location": "eastus",
    "managedBy": null,
    "name": "apim-demo-devops",
    "properties": {
      "provisioningState": "Succeeded"
    },
    "tags": null,
    "type": "Microsoft.Resources/resourceGroups"
  },

Azure CLI Run - az ad sp create-for-rbac -n Nameofapp --role contributor --scopes “subkey” --sdk-auth

Get the secret information add to Github.
Clone repo to VsCode.
Run term - dotnet new webapp.
Add newfile .github/workflows/main.yml
Edit the yaml file.
commit to repo