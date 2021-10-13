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