# Prerequisite

## PowerShell
PowerShell is a cross-platform task automation solution made up of a
command-line shell, a scripting language, and a configuration management
framework. PowerShell runs on Windows, Linux, and macOS.

* [Installing PowerShell on Windows](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows)
* [Installing PowerShell on Linux](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-linux)
* [Installing PowerShell on macOS](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-macos)
* [Installing PowerShell on ARM](https://docs.microsoft.com/en-us/powershell/scripting/install/powershell-core-on-arm)
* [Using PowerShell in Docker](https://docs.microsoft.com/en-us/powershell/scripting/install/powershell-in-docker)

### Install The Azure Az PowerShell Module

To check your PowerShell version, run the following command from within a PowerShell session:

```powershell
$PSVersionTable.PSVersion
```

PowerShell script execution policy must be set to remote signed or less
restrictive. `Get-ExecutionPolicy -List` can be used to determine the
current execution policy. For more information, see
[about_Execution_Policies](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies).

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

#### Installation

Using the [Install-Module](https://docs.microsoft.com/en-us/powershell/module/powershellget/install-module)
cmdlet is the preferred installation method for the Az PowerShell
module. Install the Az module for the current user only. This is the
recommended installation scope. This method works the same on Windows,
macOS, and Linux platforms. Run the following command from a PowerShell
session:

```powershell
Install-Module -Name Az -Scope CurrentUser -Repository PSGallery -Force
```

#### Sign In

To start working with Azure PowerShell, sign in with your Azure credentials.

```powershell
Connect-AzAccount
```

## Azure Command Line Interface (CLI)
The Azure Command Line Interface (Azure CLI) is a set of commands used
to create and manage Azure resources. The Azure CLI is available across
Azure services and is designed to get you working quickly with Azure,
with an emphasis on automation.
* [Azure Command Line Interface (CLI) Documentation](https://docs.microsoft.com/en-us/cli/azure/)



## Reference
* [Installing Various Versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell)
* [Install The Azure Az PowerShell Module](https://docs.microsoft.com/en-us/powershell/azure/install-az-ps)