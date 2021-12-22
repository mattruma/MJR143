# Introduction

## Service Principal

```bash
az ad sp create-for-rbac --name {app-name} --role contributor --scopes /subscriptions/{subscription-id}/resourceGroups/{resource-group} --sdk-auth

# Replace {subscription-id}, {resource-group} and {app-name} with the subscription, resource group and name of the WebApp
   
# The command should output a JSON object similar to this:

{
    "clientId": "<GUID>",
    "clientSecret": "<GUID>",
    "subscriptionId": "<GUID>",
    "tenantId": "<GUID>",
    (...)
}
```
