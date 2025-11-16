<p align="center">
  <img src="screenshots/mfa_banner.png" 
       alt="Project 1 — Multi-Factor Identitification Banner" width="100%">
</p>

# 🔐 Azure AD / Entra ID — MFA Enforcement Lab

**Objective:** Configure and enforce Multi-Factor Authentication (MFA) in Microsoft Entra ID using authentication method policies, targeted enforcement groups, and a registration campaign. This lab demonstrates real-world IAM administration practices essential for enterprise identity security.

---

## ✅ Overview

This project walks through enabling Microsoft Authenticator as the enforced MFA method for a targeted group, launching a registration campaign, and completing MFA registration as a user.  
All settings and flows are documented with screenshots for clarity and verification.

---

## ✅ Skills Demonstrated
- Identity & Access Management (IAM)
- Microsoft Entra ID administration
- Authentication Method Policies
- MFA Enforcement
- Registration Campaigns
- User Sign-In & Security Info Configuration
- Least Privilege Principles
- Access Governance

---

# ✅ 1. Authentication Method Policy Configuration

### ✅ Enabled Microsoft Authenticator for the MFA group  
Only the **GG-MFA-Enforced** group is allowed to register and use Microsoft Authenticator.

### Screenshot  
![Authentication Methods Policy](screenshots/auth-methods-policy.png)

---

# ✅ 2. Targeted MFA Enforcement

### ✅ Assigned enforcement to the `GG-MFA-Enforced` group  
Microsoft Authenticator was configured as a *required* method for users in this group.

---

### Screenshot  
![Authenticator Enabled for Group](screenshots/mfa-authenticator-enabled.png)

---

# ✅ 3. Registration Campaign Setup

### ✅ Registration campaign configured  
- Target: **GG-MFA-Enforced**
- Users prompted to register secure MFA methods
- Campaign forces setup upon next sign-in

### Screenshot  
![Registration Policy](screenshots/mfa-registration-policy.png)

---

# ✅ 4. User Sign-In: More Information Required

When the test user logs in, Azure AD blocks sign-in until MFA setup is completed.

### Screenshot  
![More Information Required](screenshots/mfa-more-information-required.png)

---

# ✅ 5. Microsoft Authenticator Registration Flow

The user is prompted to download the Microsoft Authenticator app and scan the QR code to register.

### Screenshot  
![Authenticator Registration Prompt](screenshots/mfa-authentication-prompt.png)

---

# ✅ 6. MFA Registration Success

Once registered, the user receives a confirmation message and MFA becomes required for future sign-ins.

### Screenshot  
![MFA Registration Success](screenshots/mfa-registration-success.png)

---

# ✅ Access Governance & Security Justification

### ✅ Why MFA Enforcement Matters  
Multi-Factor Authentication is one of the most effective ways to reduce account compromise risk.  
MFA stops:
- Password spray attacks  
- Phishing attempts  
- Brute-force authentication attempts  
- Compromised credential abuse  

---

### ✅ Why Use a Targeted Group?  
Using a group like **GG-MFA-Enforced**:
- Allows gradual rollout
- Supports pilot testing
- Ensures role-based access control (RBAC)
- Prevents accidental enforcement on Global Admins without backup creds

---

### ✅ Why Microsoft Authenticator?  
- Strongest built-in MFA option  
- Supports push notifications  
- Safer than SMS  
- Required for advanced workflows (Passwordless, Number Matching)

---

# ✅ What I Learned

- How to enforce MFA in Microsoft Entra ID  
- How to configure and target Authentication Method Policies  
- How registration campaigns work  
- How users experience MFA registration during sign-in  
- Why MFA, groups, and targeted policies matter for identity security  
- How to document IAM configurations with evidence for audits  

---

# ✅ Next Steps (Future IAM Labs)

- ✅ Conditional Access Policies  
- ✅ Passwordless Authentication  
- ✅ Joiner–Mover–Leaver Identity Lifecycle  
- ✅ Privileged Identity Management (PIM)  
- ✅ Secure Admin Accounts (Tier 0 Hardening)

---

