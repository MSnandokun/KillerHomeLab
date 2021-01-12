# NSG Flow Log Lab

Click the button below to deploy

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Felliottfieldsjr%2FKillerHomeLab%2Fmaster%2FNetwork-Security-Group-NSG-Flow%2Fazuredeploy.json)

This Templates deploys an NSG Flow Log enabled Environemnt with the following resources:

- 1 - Storage Account
- 1 - Network Security Group
- 1 - Log Analytic Workspace
- 1 - Virtual Network

Parameters that support changes
- FlowLogName. Name of NSG Flow Log
- WorkspaceLocation. Enter a Valid Azure Region for your Log Analytics Workspace based on which Cloud (AzureCloud, AzureUSGovernment, etc...) you are using.
- AdminUsername.  Enter a valid Admin Username
- AdminPassword.  Enter a valid Admin Password
- WindowsServerLicenseType.  Choose Windows Server License Type (Example:  Windows_Server or None)
- Naming Convention. Enter a name that will be used as a naming prefix for (Servers, VNets, etc) you are using.
- Vnet1ID.  Enter first 2 octets of your desired Address Space for Virtual Network 1 (Example:  10.1)
- SRV1OSVersion.  Select 2016-Datacenter (Windows 2016) or 2019-Datacenter (Windows 2019) for Server OS Version
- SRV1VMSize.  Enter a Valid VM Size based on which Region the VM is deployed.