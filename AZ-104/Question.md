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
* **Solution:** You instruct User2 to create the user accounts.
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
* **Solution:** You instruct User4 to create the user accounts.
* Does that meet the goal?

Choice

* A. Yes
* B. No

#### Correct Answer

**Answer:** B

Only a global administrator can add users to this tenant.

**Reference:** [Add or Delete Users Using Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-users-azure-active-directory)