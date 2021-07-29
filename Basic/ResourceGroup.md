# Resource Group

## Overview
A resource group is a container that holds related resources for an
Azure solution. The resource group can include all the resources for the
solution, or only those resources that you want to manage as a group.
You decide how you want to allocate resources to resource groups based
on what makes the most sense for your organization. Generally, add
resources that share the same lifecycle to the same resource group so
you can easily deploy, update, and delete them as a group.

The resource group stores metadata about the resources. Therefore, when
you specify a location for the resource group, you are specifying where
that metadata is stored. For compliance reasons, you may need to ensure
that your data is stored in a particular region.

At minimum, a **Resource Group** need to be created with a **Name** and
**Location**. The **Location** can be obtain using
[Get-AzResourceProvider](https://docs.microsoft.com/en-us/powershell/module/az.resources/get-azresourceprovider)
after [Connect-AzAccount](https://docs.microsoft.com/en-us/powershell/module/az.accounts/connect-azaccount).

## PowerShell

The `New-AzResourceGroup` cmdlet creates an Azure resource group. You
can create a resource group by using just a name and location, and then
use the New-AzResource cmdlet to create resources to add to the resource
group. To add a deployment to an existing resource group, use the
[New-AzResourceGroupDeployment](https://docs.microsoft.com/en-us/powershell/module/az.resources/new-azresourcegroupdeployment)
cmdlet. To add a resource to an existing resource group, use the
[New-AzResource](https://docs.microsoft.com/en-us/powershell/module/az.resources/new-azresource)
cmdlet. An Azure resource is a user-managed Azure entity, such as a
database server, database, or website. An Azure resource group is a
collection of Azure resources that are deployed as a unit.

```powershell
New-AzResourceGroup
   [-Name] <String>
   [-Location] <String>
   [-Tag <Hashtable>]
   [-Force]
   [-ApiVersion <String>]
   [-Pre]
   [-DefaultProfile <IAzureContextContainer>]
   [-WhatIf]
   [-Confirm]
   [<CommonParameters>]
```

### Example 1: Create an Empty Resource Group

This command creates a resource group that has no resources. You can use
the [New-AzResource](https://docs.microsoft.com/en-us/powershell/module/az.resources/new-azresource)
or [New-AzResourceGroupDeployment](https://docs.microsoft.com/en-us/powershell/module/az.resources/new-azresourcegroupdeployment)
cmdlets to add resources and deployments to this resource group.

```powershell
PS> New-AzResourceGroup -Name RG01 -Location "South Central US"
```

### Example 2: Create an Empty Resource Group Using Positional Parameters

This command creates a resource group that has no resources.

```powershell
PS> New-AzResourceGroup RG01 "South Central US"
```

### Example 3: Create a Resource Group with Tags

This command creates an empty resource group. This command is the same
as the command in [Example 1](#example-1-create-an-empty-resource-group),
except that it assigns tags to the resource group. The first tag, named
Empty, can be used to identify resource groups that have no resources.
The second tag is named Department and has a value of Marketing. You can
use a tag such as this one to categorize resource groups for
administration or budgeting.

```powershell
PS> New-AzResourceGroup -Name RG01 -Location "South Central US" -Tag @{Empty=$null; Department="Marketing"}
```

## Reference
* [Manage Azure Resource Manager Resource Groups By Using The Azure Portal](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal)
* [Manage Azure Resources By Using Azure CLI](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resources-cli)
* [Manage Azure resources By Using Azure PowerShell](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resources-powershell)
* [New-AzResourceGroup](https://docs.microsoft.com/en-us/powershell/module/az.resources/new-azresourcegroup)
* [az group](https://docs.microsoft.com/en-us/cli/azure/group)