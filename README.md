# AzureComponents_IL5_CMK_PE

Based on Bicep CARML modules which are hosted on the following github repo: https://github.com/Azure/ResourceModules

This repo provides fast deployment of the following components meeting IL5 compliance by leveraging customer managed keys (CMK) (provisioned in a keyvault) and private endpoints (leveraging associated private dns zones):

- Keyvault
- Storage
- Azure Container Registry
- AKS

To deploy Azure DevOps .yml pipelines and consolidated .bicep files are provided.

Copy of CARML modules made for simpicity around 7/1/2022 with slight refinements made for the following modules:

- AKS (to enable Disk Encryption Set linked to CMK AND central AKS private DNS zone)
- Keyvault\Keys - Added an output to support DES (Latest DES module no longer needs this)

Numerous improvements are made to the central CARML repo on a recurring basis so its recommended that you evaluate the latest version as needed. The copy is leveraged to ensure highest compatibility. There are also several CARML versioning methods that can be used instead if all your environments support this.