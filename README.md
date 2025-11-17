<p align="center">
  <img src="screenshots/mfa_banner.png" width="100%">
</p>

<h1 align="center">🛡 Project 2 — Enforce MFA for All Users</h1>
<h3 align="center">Microsoft Entra ID ▸ Zero Trust Authentication ▸ Security Hardening</h3>

---

## 📌 Overview

This project implements **Multi-Factor Authentication (MFA) enforcement** across all identities inside Microsoft Entra ID (Azure AD), simulating real IAM analyst responsibilities including:

✔ Designing and validating Conditional Access policies  
✔ Enforcing MFA without relying on end-user enrollment  
✔ Blocking insecure legacy authentication protocols  
✔ Capturing audit-ready evidence for hiring managers & security assessors  

This is **Project 2** in a **4-project Enterprise IAM portfolio series**.

---

## 📚 Table of Contents

- [Objectives](#-objectives)
- [Baseline MFA Policy](#-baseline-mfa-policy)
- [Conditional Access Configuration](#-conditional-access-configuration)
- [Legacy Authentication Blocking](#-legacy-authentication-blocking)
- [Test Validation](#-test-validation)
- [What I Learned](#-what-i-learned)
- [Next Project](#-next-project)
- [Repo Structure](#-repo-structure)

---

## 🎯 Objectives

| Objective | Outcome |
|-----------|---------|
| Require MFA for all users | Password-only sign-in eliminated |
| Block legacy auth | SMTP / IMAP / POP disabled |
| Align to Zero Trust | “Verify explicitly” implemented |
| Capture proof | Screenshot evidence for audit review |

---

## 🟦 Baseline MFA Policy

| Setting | Value |
|---------|-------|
| **Policy Name** | `01 - Require MFA for All Users` |
| **Assignment** | All Users |
| **Grant Controls** | Require MFA |
| **Mode** | Enabled |

**📸 Proof — Policy Overview**

![Policy Overview](screenshots/CA-Policy01-Overview.png)

---

## 🔐 Conditional Access Configuration

### 📋 Assignments
<details>
<summary><strong>Click to expand</strong></summary>

✔ All users included  
✖ No service principals  

![Assignments](screenshots/CA-Policy01-Assignments.png)

</details>

---

### 🎛 Conditions
<details>
<summary><strong>Click to expand</strong></summary>

🌐 Applies to all cloud apps  
🟦 No device exclusions  
🟥 No location exemptions  

![Conditions](screenshots/CA-Policy01-Conditions.png)

</details>

---

### 🛑 Grant Controls
<details>
<summary><strong>Click to expand</strong></summary>

✔ Require Multi-Factor Authentication  
⛔ No password-only authentication  

![Grant Controls](screenshots/CA-Policy01-Grant.png)

</details>

---

## 🚫 Legacy Authentication Blocking

| Policy | Action |
|--------|--------|
| `03 – Block Legacy Auth` | BLOCK |

**Why this matters**  
🔸 99% of breached accounts were not using MFA  
🔸 Legacy protocols bypass Conditional Access  
🔸 Attackers use IMAP & SMTP spray attacks

**📸 Proof**

![Block Legacy Auth](screenshots/CA-Policy03-Grant.png)

---

## 🧪 Test Validation

| Test User | Result |
|-----------|--------|
| Eddie Spark | MFA Prompt |
| Nathan Dash | MFA Prompt |
| Maverick Blaze | MFA Prompt |

🔹 Testing confirms MFA enforced **before first access attempt**  
🔹 No bypass paths remained after policy enforcement

---

## 🧠 What I Learned

✔ MFA enforcement must NOT rely on user enrollment  
✔ Legacy auth must be explicitly blocked — NOT assumed disabled  
✔ Conditional Access is the **control plane for Zero Trust**  
✔ Documentation separates **entry-level “lab builders”** from **real IAM analysts**

---

## 🧩 Where This Fits in the Portfolio

**➡ Next Project:**  
🔗 Identity Lifecycle Automation (Joiners ▸ Movers ▸ Leavers)  
https://github.com/CoachKosik/Project-3-Entra-ID-Azure-AD-Identity-Lifecycle-JML  

---

## 📂 Repo Structure

```text
azure-ad-mfa-enforcement/
│ README.md
└── screenshots/
    ├─ mfa_banner.png
    ├─ CA-Policy01-Overview.png
    ├─ CA-Policy01-Assignments.png
    ├─ CA-Policy01-Conditions.png
    ├─ CA-Policy01-Grant.png
    ├─ CA-Policy03-Grant.png
⭐ If this project helped you, please STAR the repo
🧑‍💼 Recruiters DO check GitHub activity
🧠 Full IAM portfolio → https://github.com/CoachKosik
