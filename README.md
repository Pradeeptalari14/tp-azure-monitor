# Azure Monitor & Log Analytics Studio

This repository contains the target configuration and SRE runtime files compiled by the **Azure Monitor & Log Analytics Studio** dashboard module.

## 🚀 Description
Configure enterprise diagnostic logs sinks. Generate Log Analytics workspaces templates, Kusto Query Language (KQL) SRE alert monitors, and diagnostic metrics bindings.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/monitor/monitor_rules.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-monitor.git
   cd tp-azure-monitor
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
