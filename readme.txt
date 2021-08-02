TO DEPLOY

IF NO RG
az group create --name test-mk --location "germanywestcentral"

az deployment group 
    --name testmk 
    --resource-group test-mk
    --template-file azuredeploy.json
    --parameters azuredeploy.parameters.dev.json