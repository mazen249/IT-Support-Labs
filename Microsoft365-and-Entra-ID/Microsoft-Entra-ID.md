# 🔐 Microsoft Entra ID - Identity & Access Management Lab

## 📌 Overview

This hands-on lab covers the core identity and access management concepts in Microsoft Entra ID.

The lab focuses on:

- Users
- Groups
- Roles
- Authentication
- MFA
- Identity & Access

---

## 🧪 Environment

- Microsoft Entra admin center
- Microsoft Entra ID
- Browser-based administration

---

# 1. 👤 Create a User

Created a new Microsoft Entra ID user account named `Messi`.

The account was configured with a username, display name, password, and enabled account status.

![Create Microsoft Entra ID User](../screenshots/01-create-user.png)

### Why it matters

Users represent identities within Microsoft Entra ID and are the foundation of identity and access management.

---

# 2. 👥 Create a Security Group

Created a Security Group named `IT-Group`.

The group uses **Assigned** membership and is intended for organizing IT users.

![Create Security Group](../screenshots/02-create-group.png)

### Why it matters

Groups allow administrators to manage collections of users together instead of configuring access individually for every user.

---

# 3. ➕ Add Members to the Group

Added users to the `IT-Group`, including `Messi`.

The group membership screen shows the selected users and enterprise applications.

![Group Members](../screenshots/03-group-members.png)

### Why it matters

Group-based management makes it easier to organize users and apply permissions or access policies consistently.

---

# 4. 🛡 Explore Microsoft Entra Roles

Reviewed the available administrative roles and selected the built-in **User Administrator** role.

The role allows management of users and groups, including actions such as resetting passwords for users.

![User Administrator Role](../screenshots/04-user-administrator-role.png)

### Why it matters

Microsoft Entra roles provide **role-based access control (RBAC)**.

Instead of giving every administrator full control over the directory, specific roles can provide only the administrative permissions required for a task.

> Note: The screenshot demonstrates reviewing/selecting the `User Administrator` role. It does not show an assignment of this role to `Messi`.

---

# 5. 🔑 Authentication Methods

Reviewed the Microsoft Entra **Authentication methods** policies.

The environment shows several authentication methods, including:

- Passkey (FIDO2)
- Microsoft Authenticator
- Temporary Access Pass
- Email OTP
- Software OATH tokens

Microsoft Authenticator is enabled for all users in the displayed policy.

![Authentication Methods](../screenshots/05-authentication-methods.png)

### Why it matters

Authentication methods determine how users can prove their identity when accessing Microsoft Entra-protected resources.

---

# 6. 🔐 MFA

Multi-Factor Authentication adds an additional verification factor beyond the user's password.

In this lab, Microsoft Authenticator is enabled as an available authentication method.

### Example

  text
Username + Password
        +
Microsoft Authenticator
        ↓
     Access


### Security Benefit

MFA helps protect accounts even if a password is compromised.

> The screenshot demonstrates that Microsoft Authenticator is enabled as an authentication method. It does not show a completed MFA enrollment or sign-in challenge for `Messi`.

---

# 7. 🔗 Identity & Access

The lab demonstrates how the main Microsoft Entra identity components work together:

```text
User
  ↓
Group
  ↓
Role / Permissions
  ↓
Authentication
  ↓
MFA
  ↓
Access
```

### Identity

A user such as `Messi` represents an identity in Microsoft Entra ID.

### Group

`IT-Group` provides a way to organize users together.

### Role

Administrative roles such as `User Administrator` provide specific administrative permissions.

### Authentication

Authentication methods determine how a user's identity is verified.

### MFA

Microsoft Authenticator provides an additional authentication factor.

### Access

Identity, authentication, authorization, and security controls work together to manage access to resources.

---

# 🧠 Key Concepts Learned

- Created users in Microsoft Entra ID
- Created a Security Group
- Added users to a group
- Explored Microsoft Entra administrative roles
- Reviewed the User Administrator role
- Reviewed authentication methods
- Learned the purpose of MFA
- Understood the relationship between identity, authentication, authorization, and access
- Practiced basic cloud identity and access management

---

# 🛠 Tools Used

- Microsoft Entra admin center
- Microsoft Entra ID
- Microsoft Authenticator
- Web browser

---

# 🎯 Skills Practiced

- Microsoft Entra ID
- Identity & Access Management (IAM)
- User Management
- Group Management
- Role-Based Access Control (RBAC)
- Authentication
- Multi-Factor Authentication (MFA)
- Cloud Security