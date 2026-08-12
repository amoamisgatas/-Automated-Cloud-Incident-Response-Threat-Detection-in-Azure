# 🛡️ Automated Cloud Incident Response & Threat Detection in Azure

This project demonstrates an end-to-end automated security response workflow using Microsoft Defender for Cloud and Azure Logic Apps. The architecture automatically detects misconfigured cloud resources and triggers real-time email notifications to security personnel.

---
## 📋 Prerequisites
- Active Microsoft Azure Subscription.
- Office 365 / Outlook account for notification integrations.
- Permissions to assign roles and manage Azure Logic Apps.

- ---

## 🏗️ Architecture
1. **Threat Exposure:** Storage Account created with public access enabled.
2. **Detection Engine:** Microsoft Defender for Cloud audits resource configurations.
3. **Automated Response:** Logic App (`ascalert` connector + Outlook integration) triggers upon alert generation.

---

## 🚀 Steps Implemented

- **Configured a vulnerable Storage Account with public container access:**
  ![Public Storage Container](https://github.com/user-attachments/assets/edc34fc9-5a08-4e10-94f1-d29c6479bae4)

- **Provisioned a Log Analytics Workspace for centralized logging & Monitored Security Posture:**
  ![Defender Dashboard](https://github.com/user-attachments/assets/ceea97c5-20b9-40af-ad70-83dc1b222030)

- **Built a Logic App triggered by Microsoft Defender for Cloud alerts & Integrated Office 365 / Outlook:**
  ![Logic App Workflow](https://github.com/user-attachments/assets/d5aa5e3e-df98-45f9-ae30-1332587b8b81)

- **Validated automated workflow execution:**
  ![Logic App Execution Success](https://github.com/user-attachments/assets/a22daf80-27d7-47e9-9640-d95a9883ae1e)

---

## 🛠️ Security Practices Applied
- Principle of Least Privilege in trigger selection.
- Automated SOAR (Security Orchestration, Automation, and Response) deployment.
- Verification of cloud compliance posture using Microsoft Cloud Security Benchmark.

- ---

## 🧹 Resource Cleanup
To avoid unnecessary costs and maintain a clean cloud environment, all resources within the `Security-Lab_group` resource group were deleted immediately after project validation and documentation.
