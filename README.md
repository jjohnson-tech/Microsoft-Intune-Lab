# Microsoft-Intune-Lab
Hands-on Microsoft Intune lab covering MDM enrollment configuration, compliance policy creation, endpoint security policy deployment, and app management for enterprise device management.

## Overview
Using the Microsoft Intune admin center connected to my existing Microsoft 365 tenant, this lab simulates enterprise mobile device management (MDM) tasks performed by IT administrators. The lab covers MDM enrollment configuration, compliance policy creation, endpoint security policy deployment, and app management — demonstrating how organizations manage and secure devices from the cloud without physical access.

---

## Technologies Used
- Microsoft Intune Admin Center (intune.microsoft.com)
- Microsoft Entra ID
- Microsoft Defender Antivirus
- Microsoft 365 Apps
- Microsoft 365 Business Trial Tenant

---

## Lab Environment

| Resource | Details |
|---|---|
| Tenant | jjtechlab.onmicrosoft.com |
| Admin Account | Global Administrator |
| Target Group | IT Technicians security group |
| Platform | Windows 10/11 |

---

## What I Built

**Device Enrollment** — Navigated the Intune device enrollment page and reviewed enrollment options for Windows, Apple, and Android devices. Configured MDM automatic enrollment by setting the MDM user scope to All, ensuring any device that joins the Entra ID tenant automatically enrolls into Intune management.

**Compliance Policy** — Created a Windows Compliance Baseline policy in Intune, configured minimum security requirements including BitLocker, Secure Boot, firewall, antivirus, and password complexity. Set non-compliant devices to be marked immediately and assigned the policy to the IT Technicians group, simulating enterprise device compliance enforcement.

**Endpoint Security** — Created a Microsoft Defender Antivirus policy in Intune enforcing real-time monitoring, cloud protection, behavior monitoring, and removable drive scanning across enrolled Windows devices. Assigned the policy to the IT Technicians group simulating enterprise endpoint protection configuration.

**App Deployment** — Deployed the Microsoft 365 app suite through Intune by creating an app assignment targeting the IT Technicians group, simulating enterprise app deployment where software is automatically pushed to enrolled devices without manual installation.

---

## Table of Contents

| # | Section | Description |
|---|---|---|
| 01 | [Device Enrollment](01-Device-Enrollment/README.md) | Reviewed enrollment options and configured MDM automatic enrollment for all users |
| 02 | [Compliance Policy](02-Compliance-Policy/README.md) | Created Windows Compliance Baseline with BitLocker, Secure Boot, firewall, and antivirus requirements |
| 03 | [Endpoint Security](03-Endpoint-Security/README.md) | Created Microsoft Defender Antivirus policy with real-time monitoring and cloud protection |
| 04 | [App Deployment](04-App-Deployment/README.md) | Deployed the Microsoft 365 app suite to the IT Technicians group through Intune |

---

## Key Takeaways
- Configured MDM automatic enrollment to ensure all tenant-joined devices are managed through Intune
- Created compliance policies that enforce security baselines across enrolled Windows devices
- Deployed endpoint security policies to enforce Microsoft Defender Antivirus settings without touching individual devices
- Practiced enterprise app deployment by pushing the Microsoft 365 suite to a target group automatically
- Demonstrated how cloud-based MDM allows IT teams to manage and secure devices remotely without physical access
