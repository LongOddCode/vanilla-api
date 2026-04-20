# Vanilla API App


[Azure Static Web Apps](https://docs.microsoft.com/azure/static-web-apps/overview) allows you to easily build Javascript apps in minutes. Use this repo with the [Add an API to Static Web Apps with Azure Functions](https://docs.microsoft.com/azure/static-web-apps/add-api?tabs=vanilla-javascript) article to build and customize a new static site.

This repo is used as a starter for a _very basic_ web application with an API.

## Azure CLI Command

```
az rest --method put --url  https://management.azure.com/subscriptions/0e33c8fd-9178-4f6e-aa1a-dc1dfd17c83b/resourceGroups/swa-test-samples/providers/Microsoft.Web/staticSites/xxx?api-version=2022-09-01 --body "{ 'location': 'Central US EUAP', 'name' : 'xxx', 'sku' : { 'tier': 'Standard', 'name': 'Standard' }, 'properties': { 'repositoryUrl' : 'https://github.com/cjk7989/vanilla-api', 'branch' : 'xxx', 'provider': 'GitHub', 'repositoryToken' : 'ghp_yyy', 'buildProperties' : { 'appLocation' : 'src', 'apiLocation' : 'api', 'appArtifactLocation' : '' }}}" --headers Content-Type=application/json
```
