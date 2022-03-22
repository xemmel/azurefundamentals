## Azure Fundamentals



### Arm template deployment

```powershell

$rgName = "[Your resource Group Name]";

## Create Resource Group
az group create -l westeurope -n $rgName;

## Deploy arm template (test)

az deployment group create --resource-group rg-systemate-arm --template-file .\templates\storageaccount.json --parameter .\parameters\test\storageaccount.json

```