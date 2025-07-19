# ✅ GitHub Approval Guide for TPMs – ERP Consolidation Project

[![Azure DevOps](https://img.shields.io/badge/DevOps-Azure-blue?logo=azuredevops)](https://azure.microsoft.com/services/devops)
[![Azure Data Factory](https://img.shields.io/badge/ETL-Azure_Data_Factory-0078D4?logo=microsoftazure)](https://azure.microsoft.com/services/data-factory)
[![Microsoft Dynamics 365](https://img.shields.io/badge/ERP-Dynamics_365-002050?logo=microsoft)](https://dynamics.microsoft.com)
[![SQL Server](https://img.shields.io/badge/Database-SQL_Server-CC2927?logo=microsoftsqlserver)](https://learn.microsoft.com/sql/sql-server)
[![GitHub](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com)
[![Power Platform](https://img.shields.io/badge/Power_Platform-Enabler-742774?logo=microsoftpowerpoint)](https://powerplatform.microsoft.com)
[![CI/CD](https://img.shields.io/badge/CI/CD-GitHub_Actions-blue?logo=githubactions)](https://github.com/features/actions)

---

## 📚 Table of Contents

- [📄 Summary](#-summary)
- [🔍 When to Approve a Pull Request](#-when-to-approve-a-pull-request)
- [✅ How to Approve a Pull Request](#-how-to-approve-a-pull-request)
- [📌 How to Approve or Comment on Issues](#-how-to-approve-or-comment-on-issues)
- [🔐 Role-Based Best Practices](#-role-based-best-practices)

---

## 📄 Summary

This guide supports **Technical Program Managers (TPMs)** who are temporarily handling project manager duties during the **ERP consolidation** from JD Edwards 9.2 to Microsoft Dynamics 365 (Finance & Operations). It’s designed for teams using Azure DevOps and GitHub to coordinate staging, validation, and ETL workflows.

The checklist ensures every code or configuration change passes through necessary quality gates before deployment, maintaining system integrity throughout the consolidation process.

---

## 🔍 When to Approve a Pull Request

| Review Item        | What to Check                                              |
|--------------------|------------------------------------------------------------|
| **Code Quality**   | Clear, modular, documented changes                         |
| **Linked Issue**   | References a GitHub Issue or ADO Work Item                |
| **Tests Included** | Unit tests, validation steps for ETL pipelines             |
| **No Conflicts**   | Clean merge with `main` or `dev` branch                    |
| **CI Status**      | All GitHub Actions pass (✔️ green)                         |
| **Security**       | No secrets, tokens, or credentials committed               |

---

## ✅ How to Approve a Pull Request

1. Navigate to the **Pull Requests** tab
2. Select the PR you're reviewing
3. Click the **Files Changed** tab
4. Scroll to the **Review Changes** section
5. Choose **Approve**, leave a brief note, and click **Submit review**

🛑 If uncertain, select **Request changes** and loop in the SA or DevOps Engineer.

---

## 📌 How to Approve or Comment on Issues

Use this workflow when triaging data tasks, bugs, or feature enhancements during migration.

### Steps:
- Go to the **Issues** tab in GitHub
- Open the relevant Issue
- Apply:
  - ✅ **Labels** (e.g., approved, needs review, blocked)
  - 👤 **Assignees** to delegate to a developer or QA
  - 🗂️ **Milestones** to tie it to a sprint or phase

💬 Sample comment:
> “This aligns with Sprint 2 – GL ETL staging. Proceed once PR #45 is merged and validated.”

---

## 🔐 Role-Based Best Practices

| Guideline                | Why It Matters                                          |
|--------------------------|---------------------------------------------------------|
| **Avoid self-approval**  | Enforces peer validation for higher quality             |
| **Log all approvals**    | Create a transparent audit trail in ADO or GitHub       |
| **Know the rollback plan** | Always understand the backup/branch restore path      |
| **Tag stakeholders**     | Use @mentions to alert SAs or DevOps Leads              |

---

🎯 **Pro Tip:** Convert this checklist into a GitHub Project card template or embed it in your team’s `CONTRIBUTING.md` so your whole migration team follows consistent governance.

---

