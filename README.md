# Rae Rucker

Cloud infrastructure engineer focused on Azure: backup and disaster recovery, monitoring and incident response, governance, and the automation that keeps operations repeatable.

I work at a Microsoft partner managed-services provider, operating Azure across multiple client tenants. The repositories below are independently built, tested engineering projects. Each states what has been validated locally and what hasn't been deployed yet.

[LinkedIn](https://www.linkedin.com/in/rae-rucker-929048273) · Email: `ruckerrae@gmail.com` · [Resume](https://drive.google.com/file/d/1bEpmB6ZcP0LhFx0GISZg7OY1lBAlKqeq/view?usp=sharing)

---

## Engineering focus

- Azure infrastructure and operations: networking, identity, Key Vault, governance
- Backup, disaster recovery, and recovery testing
- Monitoring, alert design, and incident response
- Infrastructure as code (Bicep) and PowerShell automation
- AKS operations and troubleshooting
- Secure delivery: OIDC, least-privilege pipelines, policy as code

---

## Featured projects

| Project | Engineering problem | Stack | Outcome |
|---|---|---|---|
| [azure-enterprise-landing-zone](https://github.com/RaeRucker/azure-enterprise-landing-zone) | New subscriptions drift without guardrails | Bicep, Azure Policy, NSG, Key Vault, Log Analytics | Hub-spoke foundation with default-deny segmentation and dev/prod policy modes; 41 tests including a negative test |
| [aks-operations-reliability](https://github.com/RaeRucker/aks-operations-reliability) | Diagnosing Kubernetes failures beyond "the pod is running" | AKS, Bicep, Cilium, kustomize, Python | Hardened cluster and workload, 6 reproducible failure scenarios, triage runbook |
| [azure-disaster-recovery-engineering](https://github.com/RaeRucker/azure-disaster-recovery-engineering) | Backups that are untested, deletable, and not tied to recovery objectives | Recovery Services, Site Recovery, Bicep | Tiered RPO/RTO design, immutable GRS vaults as code, regional failover exercise |
| [cloud-observability-incident-response](https://github.com/RaeRucker/cloud-observability-incident-response) | Alerts that are noisy, mis-severitied, or silent | Azure Monitor, KQL, Bicep, Logic Apps | Tested alert catalog with runbooks, noise controls, and a full simulated incident review |
| [secure-cloud-deployment-pipeline](https://github.com/RaeRucker/secure-cloud-deployment-pipeline) | Pipelines with stored secrets and production write access from any branch | GitHub Actions, OIDC, Bicep | Secretless, environment-gated deployment with plan, verify, and drift detection; security rules as tests |
| [azure-security-governance](https://github.com/RaeRucker/azure-security-governance) | Controls that can't be tested before they're enforced | Azure Policy, Entra ID, Conditional Access, RBAC | Unit-tested custom policies, report-only rollout, least-privilege roles, posture assessment |
| [enterprise-infrastructure-automation](https://github.com/RaeRucker/enterprise-infrastructure-automation) | One-off scripts with no tests or safeguards | PowerShell 7, Pester, Resource Graph, Microsoft Graph | 11-function module, read-only by default, 72 tests on synthetic data |

Also: [AKS-LogicMonitor-Monitoring](https://github.com/RaeRucker/AKS-LogicMonitor-Monitoring) (LM Container Helm deployment and API-throttling tuning) and [PowerShell-SQL-HealthCheck](https://github.com/RaeRucker/PowerShell-SQL-HealthCheck) (multi-instance SQL Server health reporting).

---

## Professional experience highlights

- Operate Azure for multiple client tenants through delegated (GDAP/B2B) access
- Designed Tier 1-4 backup policies with immutable, geo-redundant vaults for a client audit, including a 4-hour RPO tier
- Built a daily Azure Backup report (Logic App, Resource Graph, managed identity) requested by a client CIO
- Run Azure Site Recovery failover tests and wrote the DR runbook and report for client leadership
- Audited VMs across the client base for VM series retirements and led upgrade outreach
- Onboarded an AKS environment to enterprise monitoring in under one business day
- Reduced Azure spend by about 17% (storage optimization, lifecycle management) and alert-driven workload by about 25%

---

## Technical capabilities

| Area | Technologies |
|---|---|
| Cloud platform | Microsoft Azure |
| Infrastructure as code | Bicep |
| Automation | PowerShell, Python, Bash |
| Containers and orchestration | Kubernetes, AKS, Helm |
| Identity and security | Microsoft Entra ID, Azure RBAC, Azure Policy, Key Vault, Conditional Access |
| Monitoring | Azure Monitor, Log Analytics (KQL), LogicMonitor |
| Resilience | Azure Backup, Azure Site Recovery, SQL Server failover clustering |
| DevOps | Git, GitHub Actions, Pester, pytest |
| Systems | Windows Server, Active Directory, VMware, DNS, networking |

---

## How I work

I treat infrastructure the way I'd want to inherit it: defined in code, tested before it changes anything, observable when it fails, and documented well enough that the next engineer can recover it without me. Where a control or a recovery target hasn't been proven in a live environment, the repository says so.

---

Microsoft Certified: Azure Administrator Associate (AZ-104) · CompTIA Security+ · Microsoft Fundamentals certifications · Active Secret security clearance · Combat veteran
