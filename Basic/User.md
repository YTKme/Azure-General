# User

## Overview

Every user who needs access to Azure resources needs an Azure user
account. A user account contains all the information needed to
authenticate you during the sign-in process. Once authenticated, Azure
AD builds an access token to authorize you, and determine what resources
you can access, and what you can do with those resources.

You use the **Azure Active Directory** dashboard in the Azure portal to
work with user objects. Keep in mind that you can only work with a
single directory at a time - but you can use the
**Directory + Subscription(**) pane to switch directories. The dashboard
also has a Switch directory button in the toolbar which makes it easy to
switch to another available directory.

## PowerShell

### Read User

The `Get-AzureADUser` cmdlet gets a user from Azure Active Directory
(AD).

```powershell
Get-AzureADUser
   [-All <Boolean>]
   [-Top <Int32>]
   [-Filter <String>]
   [<CommonParameters>]
```

```powershell
Get-AzureADUser
   [-SearchString <String>]
   [-All <Boolean>]
   [<CommonParameters>]
```

```powershell
Get-AzureADUser
   -ObjectId <String>
   [-All <Boolean>]
   [<CommonParameters>]
```

#### Example 1: Get Ten Users

```powershell
PS > Get-AzureADUser -Top 10
```

### Create User

The `New-AzureADUser` cmdlet creates a user in Azure Active Directory
(Azure AD).