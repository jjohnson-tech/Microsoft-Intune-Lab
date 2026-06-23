## 02 - Compliance Policy

Compliance policies in Microsoft Intune define the minimum security requirements a device must meet to be considered compliant. If a device does not meet the requirements — such as missing BitLocker encryption or having no antivirus active — Intune marks it as non-compliant. Non-compliant devices can then be blocked from accessing company resources through Conditional Access policies. In this section a Windows Compliance Baseline policy was created and assigned to the IT Technicians group.

---

## Step 1: Navigate to Compliance Policies

Logged into the Microsoft Intune admin center at **intune.microsoft.com** and navigated to **Devices → Compliance** to access the compliance policy management page.

<img width="1907" height="422" alt="device compliance landing page" src="https://github.com/user-attachments/assets/4f0e8245-0a89-43b0-aeaa-8ff3908a780d" />


---

## Step 2: Create a New Compliance Policy

Clicked **+ Create policy** and selected the following:

- **Platform:** Windows 10 and later
- **Profile type:** Windows 10/11 compliance policy

Clicked **Create** to begin configuring the policy.

<img width="1588" height="790" alt="create a policy page " src="https://github.com/user-attachments/assets/fa31d31f-127c-4c89-a749-9567b88e0996" />


---

## Step 3: Configure Policy Basics

On the Basics tab, filled in the policy details:

- **Name:** Windows Compliance Baseline
- **Description:** Baseline compliance policy enforcing minimum security requirements for all Windows devices in the IT Technicians group

<img width="1617" height="677" alt="windows baseline compliancy page" src="https://github.com/user-attachments/assets/41a7b0c8-aec7-4c05-ad31-508b2a626a30" />


---

## Step 4: Configure Compliance Settings

On the Configuration settings tab, configured the minimum security requirements for enrolled Windows devices:

**Device Health:**
- **BitLocker:** Required — device storage must be encrypted
- **Secure Boot:** Required — device must boot into a trusted state
- **Code Integrity:** Required — only signed drivers and system files are allowed to run

**Device Properties:**
- **Minimum OS version:** 10.0.19041 (Windows 10 version 2004 or later)

**System Security:**
- **Firewall:** Required
- **Antivirus:** Required
- **Antispyware:** Required
- **Password required:** Yes
- **Minimum password length:** 8 characters
- **Password complexity:** Require digits, lowercase, uppercase, and special characters

These settings establish a security baseline that every managed Windows device must meet to be considered compliant in the tenant.

<img width="1462" height="698" alt="compliance settings for windowsp1" src="https://github.com/user-attachments/assets/f196c576-a084-4ba0-ab18-42357ce9b2e0" />
<img width="1485" height="621" alt="compliance settings for windowsp2" src="https://github.com/user-attachments/assets/9fd268c5-881c-4243-b79f-924da376c458" />


---

## Step 5: Configure Actions for Non-Compliance

On the Actions for noncompliance tab, configured what happens when a device does not meet the compliance requirements:

- **Mark device noncompliant:** Immediately — the device is flagged as non-compliant as soon as it fails any requirement

Setting the action to immediately ensures there is no grace period — any device that drops out of compliance is flagged right away so IT can investigate and remediate.

<img width="1543" height="588" alt="mark device compl" src="https://github.com/user-attachments/assets/05ce152b-1b52-44b6-9609-5778b9dedd65" />


---

## Step 6: Assign the Policy to the IT Technicians Group

On the Assignments tab, clicked **+ Add groups** and selected the **IT Technicians** security group to assign the compliance policy to all members of that group.

Assigning at the group level means any new user added to the IT Technicians group automatically falls under this compliance policy without any additional configuration.

<img width="1617" height="646" alt="it tech assigned group" src="https://github.com/user-attachments/assets/ee811210-6fa2-4a98-bc0f-dac9573f1e68" />


---

## Step 7: Review and Create the Policy

Reviewed all configured settings on the Review + create tab and clicked **Create** to deploy the Windows Compliance Baseline policy.

<img width="1627" height="757" alt="windows compliance baseline complete" src="https://github.com/user-attachments/assets/f03cf780-423f-4d3d-b32b-cad0c26984b1" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Compliance | Opened Devices → Compliance in Intune |
| Create Policy | Selected Windows 10 and later platform |
| Configure Basics | Named the policy Windows Compliance Baseline |
| Configure Settings | Enabled BitLocker, Secure Boot, firewall, antivirus, and password requirements |
| Set Non-Compliance Action | Configured devices to be marked non-compliant immediately |
| Assign to Group | Assigned policy to the IT Technicians security group |
| Create Policy | Reviewed and deployed the compliance policy |

Compliance policies are a cornerstone of enterprise device management in Intune. By defining and enforcing a security baseline across all managed devices, IT teams can ensure every device in the organization meets minimum security requirements — and automatically identify and remediate those that don't.
