**ADLSGEN2:**
-Creates an Azure Data Lake Storage Gen2 account.
- Validates mandatory and optional parameters using assertions.
- Assertions are used to verify that the configured resources match the expected values.Errors are raised if configurations do not
  align with the specified requirements.
-Ensures the application of tags and properties to maintain compliance with organizational standards
**Virtual_network:**
- Creates an Azure Virtual Network (VNet) with customizable configurations.
- Supports DNS server configuration for the VNet.
- Validates the resource properties using assertions to ensure compliance with the expected setup.
- Tags resources for better manageability and organizational alignment.
**Subnets:**
- Creates private and public subnets within a specified virtual network.
- Configurable address prefixes for each subnet.
- Supports delegation of subnets to Azure services (e.g., Databricks workspaces).
- Validation of subnet properties using assertions to ensure compliance with the expected configuration.
**Network Security Group:**
- Creates a Network Security Group (NSG) in the specified Azure Resource Group.
- Associates the NSG with both private and public subnets.
- Implements user-defined security rules.
- Includes Terraform tests to validate the module's functionality.
**Workspace:**
- Create an Azure Databricks Workspace with a custom networking setup. 
- Networking Setup, including:
- A Virtual Network (VNet).
- Public and private subnets.
- Network Security Groups (NSGs) associated with the subnets.
- Support for VNet injection to securely isolate Databricks resources within our network.
- provide the custom parameters with vnet injustion
- validates the required and optional parameters
  
  
