# AZ-104

## Topic 1

### Question 1

Your company has serval departments. Each department has a number of virtual machines (VMs).

The company has an Azure subscription that contains a resource group named RG1.

All VMs are located in RG1.

You want to associate each VM with its respective department.

What should you do?

* A. Create Azure Management Groups for each department.
* B. Create a resource group for each department.
* C. Assign tags to the virtual machines.
* D. Modify the settings of the virtual machines.

**Correct Answer:** C

**Reference:** [Use tags to organize your Azure resources and management hierarchy](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources)


### Question 2

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an Azure Active Directory (Azure AD) subscription.

You want to implement an Azure AD conditional access policy.

The policy must be configured to require members of the Global Administrators group to use Multi-Factor Authentication and an Azure AD-joined device when they connect to Azure AD from untrusted locations.

Solution: You access the multi-factor authentication page to alter the user settings.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B


### Question 3

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an Azure Active Directory (Azure AD) subscription.

You want to implement an Azure AD conditional access policy.

The policy must be configured to require members of the Global Administrators group to use Multi-Factor Authentication and an Azure AD-joined device when they connect to Azure AD from untrusted locations.

Solution: You access the Azure portal to alter the session control of the Azure AD conditional access policy.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

Reference: [Conditional Access: Require MFA for all users](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-conditional-access-policy-all-users-mfa)


### Question 4

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an Azure Active Directory (Azure AD) subscription.

You want to implement an Azure AD conditional access policy.

The policy must be configured to require members of the Global Administrators group to use Multi-Factor Authentication and an Azure AD-joined device when they connect to Azure AD from untrusted locations.

Solution: You access the Azure portal to alter the grant control of the Azure AD conditional access policy.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** A

**Reference:** [Conditional Access: Grant](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/concept-conditional-access-grant)


### Question 5

You are planning to deploy an Ubuntu Server virtual machine to your company's Azure subscription.

You are required to implement a custom deployment that includes adding a particular trusted root certification authority (CA).

Which of the following should you use to create the virtual machine?

* A. The New-AzureRmVm cmdlet.
* B. The New-AzVM cmdlet.
* C. The Create-AzVM cmdlet.
* D. The az vm create command.

**Correct Answer:** D

Once `cloud-init.txt` has been created, you can deploy the VM with `az vm create` cmdlet, using the `--custom-data` parameter to provide the full path to the `cloud-init.txt` file.

**Reference:** [Tutorial - How to use cloud-init to customize a Linux virtual machine in Azure on first boot](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/tutorial-automate-vm-deployment)


### Question 6

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company makes use of Multi-Factor Authentication for when users are not in the office. The Per Authentication option has been configured as the usage model.

After the acquisition of a smaller business and the addition of the new staff to Azure Active Directory (Azure AD) obtains a different company and adding the new employees to Azure Active Directory (Azure AD), you are informed that these employees should also make use of Multi-Factor Authentication.

To achieve this, the Per Enabled User setting must be set for the usage model.

Solution: You reconfigure the existing usage model via the Azure portal.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

Since it is not possible to change the usage model of an existing provider as it is right now, you have to create a new one and reactivate your existing server with activation credentials from the new provider.

**Reference:** [Switch usage model in Azure Multi-Factor Authentication Server](https://365lab.net/2015/04/11/switch-usage-model-in-azure-multi-factor-authentication-server/)

### Question 7

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company's Azure solution makes use of Multi-Factor Authentication for when users are not in the office. The Per Authentication option has been configured as the usage model.

After the acquisition of a smaller business and the addition of the new staff to Azure Active Directory (Azure AD) obtains a different company and adding the new employees to Azure Active Directory (Azure AD), you are informed that these employees should also make use of Multi-Factor Authentication.

To achieve this, the Per Enabled User setting must be set for the usage model.

Solution: You reconfigure the existing usage model via the Azure CLI.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

Since it is not possible to change the usage model of an existing provider as it is right now, you have to create a new one and reactivate your existing server with activation credentials from the new provider.

**Reference:** [Switch usage model in Azure Multi-Factor Authentication Server](https://365lab.net/2015/04/11/switch-usage-model-in-azure-multi-factor-authentication-server/)


### Question 8

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company's Azure solution makes use of Multi-Factor Authentication for when users are not in the office. The Per Authentication option has been configured as the usage model.

After the acquisition of a smaller business and the addition of the new staff to Azure Active Directory (Azure AD) obtains a different company and adding the new employees to Azure Active Directory (Azure AD), you are informed that these employees should also make use of Multi-Factor Authentication.

To achieve this, the Per Enabled User setting must be set for the usage model.

Solution: You create a new Multi-Factor Authentication provider with a backup from the existing Multi-Factor Authentication provider data.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** A

Since it is not possible to change the usage model of an existing provider as it is right now, you have to create a new one and reactivate your existing server with activation credentials from the new provider.

**Reference:** [Switch usage model in Azure Multi-Factor Authentication Server](https://365lab.net/2015/04/11/switch-usage-model-in-azure-multi-factor-authentication-server/)


### Question 9

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an Azure Active Directory (Azure AD) tenant named `weyland.com` that is configured for hybrid coexistence with the on-premises Active

Directory domain.

You have a server named `DirSync1` that is configured as a DirSync server.

You create a new user account in the on-premise Active Directory. You now need to replicate the user information to Azure AD immediately.

Solution: You run the `Start-ADSyncSyncCycle -PolicyType Initial` PowerShell cmdlet.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

`Initial` will perform a full sync and add the user account created but it will take time, `Delta`, will kick off a delta sync and bring only the last change, so it will be "immediately" and will fulfill the requirements.

**Reference:** [Azure AD Connect sync: Scheduler](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sync-feature-scheduler)


### Question 10

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an Azure Active Directory (Azure AD) tenant named `weyland.com` that is configured for hybrid coexistence with the on-premises Active

Directory domain.

You have a server named `DirSync1` that is configured as a DirSync server.

You create a new user account in the on-premise Active Directory. You now need to replicate the user information to Azure AD immediately.

Solution: You use Active Directory Sites and Services to force replication of the Global Catalog on a domain controller.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

On a server with Azure AD Connect installed, navigate to the Start menu and select AD Connect, then Synchronization Service.


### Question 11

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an Azure Active Directory (Azure AD) tenant named `weyland.com` that is configured for hybrid coexistence with the on-premises Active Directory domain.

You have a server named `DirSync1` that is configured as a DirSync server.

You create a new user account in the on-premise Active Directory. You now need to replicate the user information to Azure AD immediately.

Solution: You restart the NetLogon service on a domain controller.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B


### Question 12

Your company has a Microsoft Azure subscription.

The company has datacenters in Los Angeles and New York.

You are configuring the two datacenters as geo-clustered sites for site resiliency.

You need to recommend an Azure storage redundancy option.

You have the following data storage requirements:
* Data must be stored on multiple nodes.
* Data must be stored on nodes in separate geographic locations.
* Data can be read from the secondary location as well as from the primary location.

Which of the following Azure stored redundancy options should you recommend?

* A. Geo-redundant storage
* B. Read-only geo-redundant storage
* C. Zone-redundant storage
* D. Locally redundant storage

**Correct Answer:** B

RA-GRS allows you to have higher read availability for your storage account by providing "read-only" access to the data replicated to the secondary location. Once you enable this feature, the secondary location may be used to achieve higher availability in the event the data is not available in the primary region. This is an "opt-in" feature which requires the storage account be geo-replicated.

**Reference:** [Azure Storage redundancy](https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy)


### Question 13

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an azure subscription that includes a storage account, a resource group, a blob container and a file share.

A colleague named Jon Ross makes use of a solitary Azure Resource Manager (ARM) template to deploy a virtual machine and an additional Azure Storage account.

You want to review the ARM template that was used by Jon Ross.

Solution: You access the Virtual Machine blade.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

You should use the Resource Group blade.

**Reference:** [Use Azure portal to export a template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-export-template)


### Question 14

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an azure subscription that includes a storage account, a resource group, a blob container and a file share.

A colleague named Jon Ross makes use of a solitary Azure Resource Manager (ARM) template to deploy a virtual machine and an additional Azure Storage account.

You want to review the ARM template that was used by Jon Ross.

Solution: You access the Virtual Machine blade.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** A

To view a template from deployment history:
1. Go to the resource group for your new resource group. Notice that the portal shows the result of the last deployment. Select this link.
2. You see a history of deployments for the group. In your case, the portal probably lists only one deployment. Select this deployment.
3. The portal displays a summary of the deployment. The summary includes the status of the deployment and its operations and the values that you provided for parameters. To see the template that you used for the deployment, select View template.

**Reference:** [Use Azure portal to export a template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/export-template-portal)


### Question 15

**Note:** The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements.

Your company has an azure subscription that includes a storage account, a resource group, a blob container and a file share.

A colleague named Jon Ross makes use of a solitary Azure Resource Manager (ARM) template to deploy a virtual machine and an additional Azure Storage account.

You want to review the ARM template that was used by Jon Ross.

Solution: You access the Container blade.

Does the solution meet the goal?

* A. Yes
* B. No

**Correct Answer:** B

You should use the Resource Group blade

**Reference:** [Use Azure portal to export a template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/export-template-portal)


### Question 16

Your company has three virtual machines (VMs) that are included in an availability set.

You try to resize one of the VMs, which returns an allocation failure message.

It is imperative that the VM is resized.

Which of the following actions should you take?

* A. You should only stop one of the VMs.
* B. You should stop two of the VMs.
* C. You should stop all three VMs.
* D. You should remove the necessary VM from the availability set.

**Correct Answer:** C

If the VM you wish to resize is part of an availability set, then you must stop all VMs in the availability set before changing the size of any VM in the availability set.

The reason all VMs in the availability set must be stopped before performing the resize operation to a size that requires different hardware is that all running VMs in the availability set must be using the same physical hardware cluster. Therefore, if a change of physical hardware cluster is required to change the VM size then all VMs must be first stopped and then restarted one-by-one to a different physical hardware clusters.

**Reference:** [Resize virtual machines](https://azure.microsoft.com/es-es/blog/resize-virtual-machines/)


### Question 17

You have an Azure virtual machine (VM) that has a single data disk. You have been tasked with attaching this data disk to another Azure VM.

You need to make sure that your strategy allows for the virtual machines to be offline for the least amount of time possible.

Which of the following is the action you should take FIRST?

* A. Stop the VM that includes the data disk.
* B. Stop the VM that the data disk must be attached to.
* C. Detach the data disk.
* D. Delete the VM that includes the data disk.

**Correct Answer:** C

**Reference:** [How to detach a data disk from a Windows virtual machine](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/detach-disk)

**Reference:** [Attach or detach a data disk to a virtual machine in Azure DevTest Labs](https://docs.microsoft.com/en-us/azure/devtest-labs/devtest-lab-attach-detach-data-disk)


### Question 18

Your company has an Azure subscription.

You need to deploy a number of Azure virtual machines (VMs) using Azure Resource Manager (ARM) templates. You have been informed that the VMs will be included in a single availability set.

You are required to make sure that the ARM template you configure allows for as many VMs as possible to remain accessible in the event of fabric failure or maintenance.

Which of the following is the value that you should configure for the `platformFaultDomainCount` property?

* A. 10
* B. 30
* C. Min Value
* D. Max Value

**Correct Answer:** D

The number of fault domains for managed availability sets varies by region - either two or three per region.

**Reference:** [Availability options for Azure Virtual Machines](https://docs.microsoft.com/en-us/azure/virtual-machines/availability)


### Question 19

Your company has an Azure subscription.

You need to deploy a number of Azure virtual machines (VMs) using Azure Resource Manager (ARM) templates. You have been informed that the VMs will be included in a single availability set.

You are required to make sure that the ARM template you configure allows for as many VMs as possible to remain accessible in the event of fabric failure or maintenance.

Which of the following is the value that you should configure for the `platformUpdateDomainCount` property?

* A. 10
* B. 20
* C. 30
* D. 40

**Correct Answer:** B

**Reference:** [Availability sets overview](https://docs.microsoft.com/en-us/azure/virtual-machines/availability-set-overview)


### Question 20

DRAG DROP -

You have downloaded an Azure Resource Manager (ARM) template to deploy numerous virtual machines (VMs). The ARM template is based on a current VM, but must be adapted to reference an administrative password.

You need to make sure that the password cannot be stored in plain text.

You are preparing to create the necessary components to achieve your goal.

Which of the following should you create to achieve your goal? Answer by dragging the correct option from the list to the answer area.

Select and Place:

Option:
* An Azure Key Vault
* An Azure Storage Account
* Azure Active Directory (AD) Identity Protection
* An access policy
* An Azure policy
* A backup policy

Answer:
* An Azure Key Vault
* An access policy

You can use a template that allows you to deploy a simple Windows VM by retrieving the password that is stored in a Key Vault. Therefore, the password is never put in plain text in the template parameter file.

