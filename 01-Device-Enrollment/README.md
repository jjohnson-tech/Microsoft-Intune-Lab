## 01 - Device Enrollment

Device enrollment is the process of registering devices into Microsoft Intune so they can be managed, monitored, and secured from the cloud. Once a device is enrolled, Intune can push compliance policies, security settings, and apps to it without anyone physically touching the device. In this section the Intune device enrollment page was reviewed and MDM automatic enrollment was configured to ensure any device joining the Entra ID tenant is automatically enrolled into Intune management.

---

## Step 1: Navigate to the Intune Admin Center

Logged into the Microsoft Intune admin center at **intune.microsoft.com** using the Global Administrator account. The Intune admin center is the central hub for managing devices, apps, compliance policies, and endpoint security across the organization.

<img width="1882" height="847" alt="intune landing page" src="https://github.com/user-attachments/assets/4f273523-e702-4692-bb34-045a90eaa84c" />


---

## Step 2: Navigate to Device Enrollment

In the left navigation panel, clicked **Devices → Enroll devices** to access the device enrollment management page. The enrollment page provides options for enrolling Windows, Apple, and Android devices into Intune management.

<img width="1912" height="832" alt="device enrollment landing page" src="https://github.com/user-attachments/assets/772d2618-e79a-45cd-a071-50794ce7f5b8" />


---

## Step 3: Review Enrollment Options by Platform

Reviewed the enrollment options available for each device platform:

**Windows:**
- Windows Autopilot — zero-touch deployment for new devices
- Automatic enrollment — devices automatically enroll when joining Entra ID
- Bulk enrollment — enroll multiple devices at once using a provisioning package

**Apple (iOS/macOS):**
- Apple Business Manager — automated device enrollment for corporate Apple devices
- User enrollment — personal device enrollment for BYOD scenarios

**Android:**
- Android Enterprise — work profile for BYOD or fully managed corporate devices
- Samsung Knox — dedicated Samsung device management

<img width="1912" height="832" alt="device enrollment landing page" src="https://github.com/user-attachments/assets/74288395-185f-4979-a51b-0f6c3dee1b8d" />


---

## Step 4: Navigate to MDM Automatic Enrollment

Clicked on **Windows → Automatic enrollment** to configure MDM automatic enrollment for the tenant. Automatic enrollment ensures that any Windows device that joins or registers with the Entra ID tenant is automatically enrolled into Intune without requiring manual intervention from IT staff or the end user.

<img width="1867" height="800" alt="mdm device enrollment page" src="https://github.com/user-attachments/assets/ad8f18c9-fd6d-42b1-9436-cb10bb7a2547" />


---

## Step 5: Configure MDM User Scope to All

On the MDM automatic enrollment configuration page, changed the **MDM user scope** setting from **None** to **All**. Setting the scope to All means every user in the tenant — and every device they join to Entra ID — will automatically be enrolled into Intune management.

The MDM user scope options are:
- **None** — automatic enrollment is disabled
- **Some** — only users in a specific group are enrolled automatically
- **All** — every user in the tenant is enrolled automatically

For enterprise environments, setting this to All ensures no device slips through without being managed.

<img width="1912" height="846" alt="mdm all selected" src="https://github.com/user-attachments/assets/4999bbde-7962-4d1b-8e15-74450fafb812" />



---

## Step 6: Save the Configuration

Clicked **Save** to apply the MDM automatic enrollment configuration. After saving, the setting was confirmed as active — any Windows device that joins the jjtechlab tenant will now automatically enroll into Intune.

<img width="1907" height="866" alt="mdm showing saved" src="https://github.com/user-attachments/assets/5097dd21-53d6-4d8f-b7c6-946ec0a82355" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Intune | Opened Intune admin center at intune.microsoft.com |
| Navigate to Enrollment | Opened Devices → Enroll devices |
| Review Platform Options | Reviewed enrollment methods for Windows, Apple, and Android |
| Navigate to Automatic Enrollment | Selected Windows → Automatic enrollment |
| Set MDM User Scope | Changed MDM user scope from None to All |
| Save Configuration | Saved and confirmed automatic enrollment was active |

Configuring MDM automatic enrollment is a foundational Intune setup task. Setting the MDM user scope to All ensures that every device joining the tenant is automatically brought under Intune management — giving IT full visibility and control over the device fleet from day one without requiring manual enrollment steps for each device.
