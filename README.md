# azure-sentinel-arcanna-orchestrator



## Quick Deployment
Assign *Microsoft Sentinel Responder* role to the Playbook's managed identity.
Go to your Logic App > *Identity* > Add *Azure role assignments* > Add  *Microsoft Sentinel Responder* 
<br>

![image](https://user-images.githubusercontent.com/6702878/204793403-c6be8ca4-2c74-43c2-bd1e-59fb9b9e5143.png)


## Deployment with Arcanna 
If consumption plan is used make sure the ip Address from Logic Apps that region are accesible.
See https://www.microsoft.com/en-us/download/details.aspx?id=56519 and add the Whitelist.  
**Deploy with incident trigger** (recommended)

After deployment, attach this playbook to an **automation rule** so it runs when the incident is created.

[Learn more about automation rules](https://docs.microsoft.com/azure/sentinel/automate-incident-handling-with-automation-rules#creating-and-managing-automation-rules)

## Arcanna-Orchestrator 
- used to send incidents to Arcanna and await inference results 

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsiscale%2Fazure-sentinel-arcanna-orchestrator%2Fmaster%2Fazuredeploy.json)
[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsiscale%2Fazure-sentinel-arcanna-orchestrator%2Fmaster%2Fazuredeploy.json)
<br><br>


## Arcanna Feedback Loop
- used to automatically propagate feedback to Arcanna once an incident was closed in Sentinel

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsiscale%2Fazure-sentinel-arcanna-orchestrator%2Fmaster%2Farcanna-feedback-loop%2Fazuredeploy.json)
[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsiscale%2Fazure-sentinel-arcanna-orchestrator%2Fmaster%2Farcanna-feedback-loop%2Fazuredeploy.json)
<br><br>
