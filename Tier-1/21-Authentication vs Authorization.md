## Authentication

### Definition

Authentication verifies **who you are**.

### Example

```text
Username + Password
        ↓
    Who are you?
```

### When to Use

Think:

**Authentication = Who?**

---

## Authorization

### Definition

Authorization determines **what you are allowed to do**.

### Example

```text
User → Can read Storage
User → Cannot delete Storage
```










# 21. Authentication vs Authorization — Practice Questions

## 🟢 Section 1 — Basic Questions

### 1. What does authentication mean?

A. Determining what resources a user can access  
B. Verifying the identity of a user or service  
C. Encrypting data  
D. Creating a virtual network  

**Answer: B — Verifying the identity of a user or service** ✅

👉 **Authentication = Who are you?**

---

### 2. What does authorization determine?

A. Whether a user is who they claim to be  
B. Whether a user's password is correct  
C. What actions or resources an authenticated user is allowed to access  
D. Whether a user has MFA enabled  

**Answer: C — What actions or resources an authenticated user is allowed to access** ✅

👉 **Authorization = What are you allowed to do?**

---

### 3. Which statement best describes authentication?

A. Checking permissions  
B. Verifying identity  
C. Assigning roles  
D. Creating subscriptions  

**Answer: B — Verifying identity** ✅

---

### 4. Which statement best describes authorization?

A. Verifying a user's identity  
B. Verifying a password  
C. Determining access permissions  
D. Verifying an MFA code  

**Answer: C — Determining access permissions** ✅

---

### 5. A user enters a username and password to sign in to Azure. What process is occurring?

A. Authorization  
B. Authentication  
C. Governance  
D. Encryption  

**Answer: B — Authentication** ✅

---

### 6. After successfully signing in, Azure determines whether the user can create a virtual machine. What process is this?

A. Authentication  
B. Authorization  
C. Authentication and encryption  
D. Availability  

**Answer: B — Authorization** ✅

---

### 7. Which question is answered by authentication?

A. What can you access?  
B. What permissions do you have?  
C. Who are you?  
D. Which subscription should you use?  

**Answer: C — Who are you?** ✅

---

### 8. Which question is answered by authorization?

A. Who are you?  
B. Are you allowed to perform this action?  
C. What is your password?  
D. Are you using MFA?  

**Answer: B — Are you allowed to perform this action?** ✅

---

# 🟡 Section 2 — Microsoft Entra ID Questions

### 9. Which Azure service provides identity and access management capabilities?

A. Azure Storage  
B. Microsoft Entra ID  
C. Azure Virtual Network  
D. Azure Monitor  

**Answer: B — Microsoft Entra ID** ✅

📌 **Remember:**  
**Microsoft Entra ID = Identity and access management**

---

### 10. A company wants employees to sign in to Microsoft Azure using their organizational identities. Which service should they use?

A. Azure DNS  
B. Microsoft Entra ID  
C. Azure Load Balancer  
D. Azure Storage  

**Answer: B — Microsoft Entra ID** ✅

---

### 11. Which Azure service can authenticate users and applications?

A. Microsoft Entra ID  
B. Azure Virtual Network  
C. Azure Firewall  
D. Azure Monitor  

**Answer: A — Microsoft Entra ID** ✅

---

### 12. A user is required to provide a password and a code sent to their phone when signing in. What security feature is being used?

A. RBAC  
B. MFA  
C. NSG  
D. VNet Peering  

**Answer: B — MFA** ✅

👉 **MFA = Multi-Factor Authentication**

---

### 13. Which of the following is an example of authentication?

A. Giving a user the Contributor role  
B. Checking a user's password  
C. Allowing a user to create VMs  
D. Assigning a user to a resource group  

**Answer: B — Checking a user's password** ✅

---

### 14. Which of the following is an example of authorization?

A. Entering a password  
B. Providing an MFA code  
C. Assigning the Contributor role to a user  
D. Signing in with a username  

**Answer: C — Assigning the Contributor role to a user** ✅

---

# 🟠 Section 3 — RBAC Questions

### 15. What is Azure role-based access control (Azure RBAC) primarily used for?

A. Verifying user identities  
B. Controlling access to Azure resources  
C. Encrypting virtual machines  
D. Monitoring applications  

**Answer: B — Controlling access to Azure resources** ✅

---

### 16. A user has successfully authenticated to Azure. The company wants the user to manage virtual machines but not modify networking resources. What should the company use?

A. MFA  
B. Azure RBAC  
C. Microsoft Entra ID authentication  
D. Azure DNS  

**Answer: B — Azure RBAC** ✅

👉 **RBAC = Authorization**

---

### 17. Which Azure RBAC role generally provides permissions to manage resources but does not allow assigning access to others?

A. Owner  
B. Contributor  
C. Reader  
D. User Access Administrator  

**Answer: B — Contributor** ✅

📌 **Exam Point:**

- **Owner** → Can manage resources + assign access
- **Contributor** → Can manage resources but cannot assign RBAC access
- **Reader** → Can view resources but cannot modify them

---

### 18. A user needs permission to view Azure resources but not modify them. Which role is most appropriate?

A. Owner  
B. Contributor  
C. Reader  
D. User Access Administrator  

**Answer: C — Reader** ✅

---

### 19. A user needs to manage Azure resources and assign access permissions to other users. Which role is appropriate?

A. Reader  
B. Contributor  
C. Owner  
D. Guest  

**Answer: C — Owner** ✅

---

### 20. Which of the following is an example of authorization?

A. A user enters their password  
B. A user provides an MFA code  
C. A user is assigned the Reader role on a resource group  
D. Microsoft Entra ID verifies the user's identity  

**Answer: C — A user is assigned the Reader role on a resource group** ✅

---

# 🔴 Section 4 — Scenario-Based Exam Questions

### 21. A company requires users to verify their identity using a password and a mobile application before accessing Azure resources.

What is being implemented?

A. Authorization  
B. Multi-factor authentication  
C. RBAC  
D. Resource locking  

**Answer: B — Multi-factor authentication** ✅

---

### 22. A user successfully signs in to Azure but receives an error when attempting to delete a virtual machine.

What is the most likely reason?

A. Authentication failed  
B. The user does not have sufficient authorization  
C. The user's username is invalid  
D. MFA is disabled  

**Answer: B — The user does not have sufficient authorization** ✅

🔥 **Very Important Exam Scenario**

The user **successfully signed in** → Authentication succeeded.

The user **cannot perform an action** → Authorization / permissions issue.

---

### 23. An administrator wants to ensure that only authorized users can manage resources in a particular resource group.

Which feature should the administrator use?

A. Azure RBAC  
B. MFA  
C. Microsoft Entra authentication only  
D. Azure DNS  

**Answer: A — Azure RBAC** ✅

---

### 24. A company wants to require users to provide two forms of verification when signing in to Microsoft cloud services.

Which feature should the company configure?

A. Azure RBAC  
B. MFA  
C. Azure Policy  
D. Resource Locks  

**Answer: B — MFA** ✅

---

### 25. A user has been successfully authenticated using Microsoft Entra ID. The user can view a storage account but cannot delete it.

What does this demonstrate?

A. Authentication without authorization  
B. Authorization without authentication  
C. Encryption without authentication  
D. Authentication failure  

**Answer: A — Authentication without authorization** ✅

---

# ⭐ Quick Exam Reminder

**Authentication → Who are you?**

**Authorization → What are you allowed to do?**

**Microsoft Entra ID → Identity and access management**

**MFA → Multiple verification factors**

**Azure RBAC → Controls access to Azure resources**

**Owner → Manage resources + assign access**

**Contributor → Manage resources, but cannot assign RBAC access**

**Reader → View resources only**
### When to Use

Think:

**Authorization = What can you do?**
