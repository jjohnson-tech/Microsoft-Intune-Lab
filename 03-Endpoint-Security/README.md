## 03 - Endpoint Security

Endpoint security policies in Microsoft Intune allow IT administrators to configure and enforce security settings on enrolled devices without touching them individually. In this section a Microsoft Defender Antivirus policy was created in Intune to enforce real-time monitoring, cloud protection, behavior monitoring, and removable drive scanning across enrolled Windows devices. The policy was assigned to the IT Technicians group simulating enterprise endpoint protection configuration.

---

## Step 1: Navigate to Endpoint Security

Logged into the Microsoft Intune admin center at **intune.microsoft.com** and navigated to **Endpoint security** in the left navigation panel to access the endpoint security policy management page.

<img width="1912" height="857" alt="endpoint landing page" src="https://github.com/user-attachments/assets/7fa1a95a-f223-44e2-b1b3-bf405a7b4aee" />


---

## Step 2: Navigate to Antivirus

Clicked **Antivirus** under the Endpoint security section to access the antivirus policy management page. This is where Microsoft Defender Antivirus policies are created and managed for enrolled Windows devices.

<img width="1912" height="707" alt="endpoint antivirus landing page" src="https://github.com/user-attachments/assets/277fa676-a78f-487e-ab67-2cbc95ae39a9" />


---

## Step 3: Create a New Antivirus Policy

Clicked **+ Create policy** and configured the platform and profile:

- **Platform:** Windows 10, Windows 11, and Windows Server
- **Profile:** Microsoft Defender Antivirus

Clicked **Create** to begin configuring the policy.

<img width="1266" height="722" alt="endpoint create pane page" src="https://github.com/user-attachments/assets/3df8a6cf-5fd4-4ba3-837f-a58fc42aae09" />


---

## Step 4: Configure Policy Basics

On the Basics tab, filled in the policy details:

- **Name:** Windows Defender Antivirus Baseline
- **Description:** Antivirus policy enforcing Microsoft Defender settings across enrolled Window devices in the JJ Tech Lab envrionment
- 
<img width="1585" height="791" alt="endpoint creat a policy basics" src="https://github.com/user-attachments/assets/55029388-5692-4e2a-95a1-f40d3db93b4b" />

---

## Step 5: Configure Antivirus Settings

On the Configuration settings tab, configured the Microsoft Defender Antivirus settings to enforce across all enrolled devices:

**Real-time protection:**
- **Turn on real-time protection:** Yes — continuously monitors files and processes for threats
- **Enable on access protection:** Yes — scans files when they are opened or downloaded
- **Monitor file and program activity on your computer:** Yes

**Cloud protection:**
- **Turn on cloud-delivered protection:** Yes — sends suspicious file data to Microsoft's cloud for faster threat analysis
- **Block at first sight:** Yes — blocks new malware immediately based on cloud analysis before a definition update is released

**Behavior monitoring:**
- **Turn on behavior monitoring:** Yes — detects suspicious behavior patterns even from previously unknown threats

**Removable drives:**
- **Scan removable drives during full scan:** Yes — includes USB drives and external storage in full scans

These settings ensure every enrolled device has consistent, enterprise-grade antivirus protection enforced by policy rather than relying on individual users to configure their own settings.

<img width="1517" height="706" alt="enpoint policy config settings page" src="https://github.com/user-attachments/assets/86c08c31-23cd-4512-b58f-9077bd5486c9" />


## Step 6: Assign the Policy to the IT Technicians Group

On the Assignments tab, clicked **+ Add groups** and selected the **IT Technicians** security group to assign the antivirus policy to all members of that group.

<img width="1610" height="705" alt="endpoint role assignment it" src="https://github.com/user-attachments/assets/b696f575-cd4f-4c7a-b2be-d0c0672f42c1" />


---

## Step 7: Review and Create the Policy

Reviewed all configured settings on the Review + create tab and clicked **Create** to deploy the Windows Defender Antivirus Baseline policy. Confirmed the policy appeared in the Antivirus policies list as active.

<img width="1562" height="753" alt="endpoint security policy done" src="https://github.com/user-attachments/assets/f59d6d4c-918a-4675-8b18-46ec2e66d249" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Endpoint Security | Opened Endpoint security in the Intune admin center |
| Navigate to Antivirus | Opened the Antivirus policy management page |
| Create Policy | Selected Windows platform and Microsoft Defender Antivirus profile |
| Configure Basics | Named the policy Windows Defender Antivirus Baseline |
| Configure Settings | Enabled real-time protection, cloud protection, behavior monitoring, and removable drive scanning |
| Assign to Group | Assigned policy to the IT Technicians security group |
| Create Policy | Reviewed and deployed the antivirus policy |

Endpoint security policies in Intune remove the dependency on individual users to configure their own security settings. By pushing a standardized Defender Antivirus policy to all enrolled devices through the IT Technicians group, IT ensures every managed device has consistent protection — enforced from the cloud without requiring physical access to any device.
