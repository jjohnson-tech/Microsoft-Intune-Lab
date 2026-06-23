## 04 - App Deployment

App deployment in Microsoft Intune allows IT administrators to push applications to enrolled devices automatically without requiring users to manually download or install anything. Apps can be assigned as Required — meaning they install automatically — or Available — meaning users can choose to install them from the Company Portal. In this section the Microsoft 365 app suite was deployed through Intune and assigned to the IT Technicians group, simulating how enterprise app deployment works in a managed device environment.

---

## Step 1: Navigate to Apps

Logged into the Microsoft Intune admin center at **intune.microsoft.com** and navigated to **Apps → All apps** to access the app management page.

<img width="1902" height="501" alt="all apps overview" src="https://github.com/user-attachments/assets/0fe805bb-8fe2-4cf5-b5a3-f86cd990ca4a" />


---

## Step 2: Add a New App

Clicked **+ Add** to begin adding a new app to Intune. On the Select app type panel, selected **Microsoft 365 Apps for Windows 10 and later** under the Microsoft 365 Apps section.

Clicked **Select** to proceed.



---

## Step 3: Configure App Suite Information

On the App suite information tab, reviewed the pre-populated details for the Microsoft 365 app suite:

- **Name:** Microsoft 365 Apps
- **Description:** Microsoft 365 app suite deployed to all enrolled Windows devices
- **Publisher:** Microsoft
- **Category:** Productivity

<img width="1488" height="698" alt="app suite info for app" src="https://github.com/user-attachments/assets/4803b306-97e0-4fdf-a8df-06341d455755" />


---

## Step 4: Configure App Suite Settings

On the App suite settings tab, configured how the Microsoft 365 apps will be installed on enrolled devices:

- **Update channel:** Monthly Enterprise Channel — receives monthly updates with a predictable schedule
- **Apps to install:** Selected the full Microsoft 365 suite including Word, Excel, PowerPoint, Outlook, Teams, and OneNote
- **Architecture:** 64-bit
- **Remove other versions:** Yes — removes any older versions of Office installed on the device before deploying the new suite

<img width="1610" height="735" alt="config app suite" src="https://github.com/user-attachments/assets/accb14fc-a589-4ca2-abd2-70a0149f5046" />


---

## Step 5: Assign the App to the IT Technicians Group

On the Assignments tab, clicked **+ Add group** under the **Required** section and selected the **IT Technicians** security group.

Assigning the app as **Required** means the Microsoft 365 suite will automatically install on any enrolled device belonging to a member of the IT Technicians group — no user action needed. The two assignment types are:

- **Required** — app installs automatically on enrolled devices
- **Available for enrolled devices** — app appears in the Company Portal for users to install manually

<img width="1546" height="480" alt="it tech role assignment app" src="https://github.com/user-attachments/assets/870f85eb-3feb-4966-8331-b4ba158ccf85" />


---

## Step 6: Review and Create the App Deployment

Reviewed all configured settings on the Review + create tab and clicked **Create** to deploy the Microsoft 365 app suite. Confirmed the app appeared in the All Apps list with the assignment targeting the IT Technicians group.

<img width="1612" height="782" alt="app done  age" src="https://github.com/user-attachments/assets/c43ad98f-71da-4e1a-9f8f-703c8b628f8d" />


---

## Summary

| Task | Action |
|---|---|
| Navigate to Apps | Opened Apps → All apps in the Intune admin center |
| Add New App | Selected Microsoft 365 Apps for Windows 10 and later |
| Configure App Info | Reviewed app suite name, description, and publisher |
| Configure Settings | Set update channel, architecture, and app selection |
| Assign to Group | Assigned app as Required to the IT Technicians group |
| Create Deployment | Reviewed and deployed the Microsoft 365 app suite |

App deployment through Intune eliminates the need for IT staff to manually install software on individual devices. By assigning the Microsoft 365 suite as Required to the IT Technicians group, the apps automatically install on every enrolled device in that group — saving time, reducing errors, and ensuring every team member has the same standardized software environment from day one.
