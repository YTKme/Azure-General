# AZ-104

## Topic 1

**Note:** This question is part of a series of questions that present
the same scenario. Each question in the series contains a unique
solution that might meet the stated goals. Some question sets might have
more than one correct solution, while others might not have a correct
solution.

After you answer a question in this section, you will NOT be able to
return to it. As a result, these questions will not appear in the review
screen.

### Question 1

You have an Azure subscription that contains the following users in an
Azure Active Directory tenant named **contoso.onmicrosoft.com**:

| Name  | Role                 | Scope                  |
|-------|----------------------|------------------------|
| User1 | Global Administrator | Azure Active Directory |
| User2 | Global Administrator | Azure Active Directory |
| User3 | User Administrator   | Azure Active Directory |
| User4 | Owner                | Azure Subscription     |

* **User1** creates a new Azure Active Directory tenant named **external.contoso.onmicrosoft.com**.
* You need to create new user accounts in **external.contoso.onmicrosoft.com**.
* **Solution:** You instruct **User2** to create the user accounts.
* Does that meet the goal?

Choice
* A. Yes
* B. No

#### Correct Answer

**Answer:** A

Only a global administrator can add users to this tenant.

**Reference:** [Add or Delete Users Using Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-users-azure-active-directory)

### Question 2

You have an Azure subscription that contains the following users in an
Azure Active Directory tenant named **contoso.onmicrosoft.com**:

| Name  | Role                 | Scope                  |
|-------|----------------------|------------------------|
| User1 | Global Administrator | Azure Active Directory |
| User2 | Global Administrator | Azure Active Directory |
| User3 | User Administrator   | Azure Active Directory |
| User4 | Owner                | Azure Subscription     |

* **User1** creates a new Azure Active Directory tenant named **external.contoso.onmicrosoft.com**.
* You need to create new user accounts in **external.contoso.onmicrosoft.com**.
* **Solution:** You instruct **User4** to create the user accounts.
* Does that meet the goal?

Choice

* A. Yes
* B. No

#### Correct Answer

**Answer:** B

Only a global administrator can add users to this tenant.

**Reference:** [Add or Delete Users Using Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-users-azure-active-directory)

### Question 3

You have an Azure subscription that contains the following users in an
Azure Active Directory tenant named **contoso.onmicrosoft.com**:

| Name  | Role                 | Scope                  |
|-------|----------------------|------------------------|
| User1 | Global Administrator | Azure Active Directory |
| User2 | Global Administrator | Azure Active Directory |
| User3 | User Administrator   | Azure Active Directory |
| User4 | Owner                | Azure Subscription     |

* **User1** creates a new Azure Active Directory tenant named **external.contoso.onmicrosoft.com**.
* You need to create new user accounts in **external.contoso.onmicrosoft.com**.
* **Solution:** You instruct **User3** to create the user accounts.
* Does that meet the goal?

Choice

* A. Yes
* B. No

**Answer:** B

Only a global administrator can add users to this tenant.

**Reference:** [Add or Delete Users Using Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-users-azure-active-directory)

### Question 4

You have an Azure subscription named **Subscription1** that contains a
resource group named **RG1**. In **RG1**, you create an internal load
balancer named LB1 and a public load balancer named **LB2**. You need to
ensure that an administrator named **Admin1** can manage **LB1** and
**LB2**. The solution must follow the principle of least privilege.

Which role should you assign to **Admin1** for each task? To answer,
select the appropriate options in the answer area.

**NOTE:** Each correct selection is worth one point.

#### Correct Answer

* To add a backend pool to **LB1**: Network Contributor on **LB1**
* To add a health probe to **LB2**: Network Contributor on **LB2**

The **Network Contributor** role lets you manage networks, but not
access them.

**Reference:** [Azure Built-In Roles](https://docs.microsoft.com/en-us/azure/role-based-access-control/built-in-roles)

### Question 5

You have an Azure subscription that contains an Azure Active Directory
(Azure AD) tenant named **contoso.com** and an Azure Kubernetes Service
(AKS) cluster named **AKS1**.

* An administrator reports that she is unable to grant access to **AKS1** to the users in **contoso.com**.
* You need to ensure that access to **AKS1** can be granted to the **contoso.com** users.
* What should you do first?

Choice
* A. From **contoso.com**, modify the Organization relationships settings.
* B. From **contoso.com**, create an OAuth 2.0 authorization endpoint.
* C. Recreate **AKS1**.
* D. From **AKS1**, create a namespace.

#### Correct Answer

**Answer:** B

**Reference:** [Kubernetes Authenticating](https://kubernetes.io/docs/reference/access-authn-authz/authentication/)

### Question 6

You have a Microsoft 365 tenant and an Azure Active Directory (Azure AD)
tenant named **contoso.com**. You plan to grant three users named
**User1**, **User2**, and **User3** access to a temporary Microsoft
SharePoint document library named **Library1**. You need to create
groups for the users. The solution must ensure that the groups are
deleted automatically after 180 days.

Which two groups should you create? Each correct answer presents a
complete solution.

**NOTE:** Each correct selection is worth one point.

Choice
* A. a Microsoft 365 group that uses the Assigned membership type
* B. a Security group that uses the Assigned membership type
* C. a Microsoft 365 group that uses the Dynamic User membership type
* D. a Security group that uses the Dynamic User membership type
* E. a Security group that uses the Dynamic Device membership type

#### Correct Answer

**Answer:** A, C

You can set expiration policy only for Office 365 groups in Azure Active
Directory (Azure AD).

**Note:** With the increase in usage of Office 365 Groups,
administrators and users need a way to clean up unused groups.
Expiration policies can help remove inactive groups from the system and
make things cleaner.

When a group expires, all of its associated services (the mailbox,
Planner, SharePoint site, etc.) are also deleted. You can set up a rule
for dynamic membership on security groups or Office 365 groups.

**Incorrect Answer:** B, D, E

You can set expiration policy only for Office 365 groups in Azure Active
Directory (Azure AD).

**Reference:** [Microsoft 365 Group Expiration Policy](https://docs.microsoft.com/en-us/microsoft-365/solutions/microsoft-365-groups-expiration-policy)

