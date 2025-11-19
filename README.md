<p align="center">
  <img src="screenshots/project_2_banner.png" width="100%">
</p>

<h1 align="center">🛡 Project 2 — Enforce Multi-Factor Authentication (MFA)</h1>
<h3 align="center">Microsoft Entra ID ▸ Zero Trust Authentication ▸ Enterprise IAM Lab</h3>

---

#### Authentication Methods · Registration Campaign · MFA Policy Testing

> **TL;DR:** Enforced MFA across all identities using Authentication Methods, Conditional Access, and real user registration flows.  
> **Focus:** modern authentication, legacy auth blocking, Zero Trust enforcement.

---

## 🔵 Why This Project Matters to IAM Hiring Managers

MFA enforcement is one of the **highest-impact IAM controls**, and this project demonstrates that I can implement it the right way — using Conditional Access and modern Authentication Methods rather than outdated legacy settings.

What this proves I can do:

- **Configure Authentication Methods policies** to enforce Microsoft Authenticator correctly  
- Deploy and test a **Registration Campaign** for real users  
- Implement **Conditional Access** for enforceable MFA requirements  
- **Block legacy authentication protocols**, which are responsible for the majority of compromised accounts  
- Validate policies through real **user sign-in testing**, ensuring enforcement actually works  
- Provide **clear, audit-friendly documentation** for security reviews or compliance teams

This aligns with the expectations for:

- IAM Analysts  
- Identity & Access Engineers  
- Security Operations (SecOps) IAM roles  
- Zero Trust / Authentication specialists

---

## 📚 Table of Contents

- [Objectives](#-objectives)
- [Authentication Method Policies](#-authentication-method-policies)
- [Group-Targeted MFA Enforcement](#-group-targeted-mfa-enforcement)
- [Registration Campaign](#-registration-campaign-required-enrollment)
- [User Registration Experience](#-user-registration-experience)
- [MFA Authentication Test](#-mfa-authentication-test)
- [What I Learned](#-what-i-learned)
- [Next Project](#-next-project--identity-lifecycle-jml)
- [Repo Structure](#-repo-structure)

---

## 🎯 Objectives

| Objective | Outcome |
|-----------|---------|
| Enforce MFA | Microsoft Authenticator required |
| Control rollout | Enforcement limited to IAM MFA group |
| Verify Zero Trust | “Verify explicitly” enforced at sign-in |
| Capture audit evidence | Screenshots included for every control |

---

## 🔐 Authentication Method Policies

<details>
<summary><strong>📸 Authentication Method Policy View</strong></summary>

![Authentication Method Policy](screenshots/auth-methods-policy.png)

</details>

---

## 🎯 Group-Targeted MFA Enforcement

**Target Group:** `GG-MFA-Enforced`  
**Authentication Method:** Microsoft Authenticator  
**Mode:** Enabled

<details>
<summary><strong>📸 Microsoft Authenticator Policy Targeting</strong></summary>

![Microsoft Authenticator Settings](screenshots/mfa-authenticator-enabled.png)  
![Microsoft Authenticator Settings 2](screenshots/mfa-authenticator-enabled-2.png)

</details>

---

## 🏁 Registration Campaign (Required Enrollment)

<details>
<summary><strong>📸 Registration Campaign Settings</strong></summary>

![Registration Campaign](screenshots/mfa-registration-policy.png)

</details>

---

## 👤 User Registration Experience

<details>
<summary><strong>📸 User prompted for more information</strong></summary>

![More Information Required](screenshots/mfa-more-information-required.png)

</details>

<details>
<summary><strong>📸 Authenticator success confirmation</strong></summary>

![Registration Success](screenshots/mfa-registration-success.png)

</details>

---

## 🧪 MFA Authentication Test

**User attempts sign-in → Forced MFA challenge**

<details>
<summary><strong>📸 Authentication Prompt</strong></summary>

![Approve MFA Sign-In](screenshots/mfa-authentication-prompt.png)

</details>

---

## 🧠 What I Learned

✔ MFA MUST be enforced — **not just offered**  
✔ Group-based enforcement enables controlled rollout  
✔ Authentication Methods policy now replaces legacy MFA portal  
✔ Documentation is a **core IAM job skill**, not an afterthought  
✔ Audit evidence must show **policy → registration → successful enforcement**

---

## ➤ Next Project — Identity Lifecycle (JML)

**Joiners ▸ Movers ▸ Leavers ▸ Full Access Proven**

🔗 [Project 3 — Microsoft Entra ID Identity Lifecycle (JML)](https://github.com/CoachKosik/Project-3-Microsoft-Entra-ID-Identity-Lifecycle-JML/blob/main/README.md)

---

## 📂 Repo Structure

```text
entra-id-mfa-enforcement/
│ README.md
└── screenshots/
    ├─ mfa_banner.png
    ├─ auth-methods-policy.png
    ├─ mfa-authenticator-enabled.png
    ├─ mfa-authenticator-enabled-2.png
    ├─ mfa-registration-policy.png
    ├─ mfa-more-information-required.png
    ├─ mfa-registration-success.png
    ├─ mfa-authentication-prompt.png
```

---

## 🧩 Skills Demonstrated
- Microsoft Entra ID Authentication Methods policy configuration
- MFA enforcement using Conditional Access (Require MFA)
- End-user MFA registration flow testing (Authenticator app)
- Registration Campaign deployment & enrollment validation
- Legacy authentication blocking (POP/IMAP/SMTP hardening)
- Modern authentication alignment with Zero Trust
- Audit-ready MFA documentation & policy evidence collection

---

⭐ **If this project helped you, please STAR the repo**<br>
🧑‍💻 Full IAM Portfolio → https://github.com/CoachKosik<br>
🧠 *Proof-based IAM > text-only IAM*
