
# HurkSystems – Azure Cloud Infrastructure

## Project Overview

HurkSystems is a fictional organisation used to simulate the design, implementation and management of an enterprise Microsoft Azure environment.

This project demonstrates practical cloud engineering skills through the implementation of cloud infrastructure, identity management, security, governance and automation using Microsoft Azure.

The project also supports hands-on learning aligned with the Microsoft Azure Administrator (AZ-104) certification.

## Project Objectives

- Establish a secure Azure environment.
- Implement cloud governance and cost management.
- Configure identity and access management.
- Apply the principle of least privilege.
- Design and deploy cloud networking.
- Deploy and manage compute and storage resources.
- Implement infrastructure monitoring and security.
- Automate infrastructure deployment using Terraform.
- Implement CI/CD pipelines for infrastructure deployment.
- Maintain technical documentation aligned with industry best practices.

## Environment

| Component | Configuration |
|---|---|
| Organisation | HurkSystems |
| Cloud provider | Microsoft Azure |
| Subscription | `sub-hurksystems-sandbox-001` |
| Subscription type | Pay-As-You-Go |
| Environment | Sandbox |
| Identity provider | Microsoft Entra ID |
| Tenant name | HurkSystems |
| Primary domain | `hurkssystems.onmicrosoft.com` |
| Tenant licence | Microsoft Entra ID Free |
| Identity model | Cloud-only |
| Security Defaults | Enabled |
| Monthly budget | A$1.00 AUD |
| Budget scope | Billing profile |

## Project Progress

- [x] Azure subscription configuration
- [x] Budget and cost management
- [x] Tenant configuration
- [ ] Identity and access management
- [ ] Azure governance
- [ ] Resource organisation
- [ ] Virtual networking
- [ ] Compute and storage
- [ ] Monitoring and security
- [ ] Infrastructure as Code
- [ ] CI/CD and automation

## Documentation

| Phase | Documentation | Status |
|---|---|---|
| 01 | [Subscription and Cost Management](docs/01-subscription-and-cost-management.md) | Completed |
| 02 | [Tenant Configuration](docs/02-tenant-configuration.md) | Completed |
| 03 | Identity and Access Management | In Progress |
| 04 | Azure Governance | Planned |
| 05 | Resource Organisation | Planned |
| 06 | Virtual Networking | Planned |
| 07 | Compute and Storage | Planned |
| 08 | Monitoring and Security | Planned |
| 09 | Infrastructure as Code | Planned |
| 10 | CI/CD and Automation | Planned |

## Security

The HurkSystems environment is designed with security and least-privilege access as foundational principles.

The following identity security controls have been implemented:

- Microsoft Entra ID Security Defaults.
- Microsoft Authenticator registration for the daily administrator.
- Separate daily and emergency administrative accounts.
- Least-privilege Microsoft Entra directory role assignments.
- Disabled Azure resource access elevation for the daily administrator.

Additional security and governance controls will be introduced throughout subsequent project phases.

Sensitive account information and environment identifiers are redacted from publicly available screenshots.

## Cost Management

A monthly budget of A$1.00 AUD has been configured at the billing profile scope to monitor expenditure and provide email notifications at defined thresholds.

Budget notifications are configured at the following actual expenditure thresholds:

| Threshold | Alert type |
|---|---|
| 1% | Actual cost |
| 50% | Actual cost |
| 80% | Actual cost |
| 100% | Actual cost |

Azure budgets provide notifications rather than hard spending limits. Additional governance controls will be introduced to help reduce the risk of unexpected charges.

Resources will be deployed with consideration for cost, operational requirements and available Azure free service allowances.

## Technologies

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud infrastructure and services |
| Microsoft Entra ID | Identity and access management |
| Azure RBAC | Resource access control |
| Azure Policy | Governance and compliance |
| Azure Cost Management | Budgeting and expenditure monitoring |
| Azure Virtual Network | Cloud networking |
| Azure Virtual Machines | Compute infrastructure |
| Azure Storage | Cloud storage services |
| Azure Monitor | Infrastructure monitoring |
| Terraform | Infrastructure as Code |
| GitHub | Version control and technical documentation |
| GitHub Actions | CI/CD and infrastructure automation |

Technologies are introduced progressively throughout the project phases.

## Design Principles

- Security by design
- Principle of least privilege
- Cost optimisation
- Consistent resource naming
- Infrastructure standardisation
- Automation and repeatability
- Maintainable technical documentation

## Disclaimer

HurkSystems is a fictional organisation. This environment is intended for professional development, technical experimentation and demonstration purposes.

The environment is a sandbox and is not intended to host production workloads. Configuration decisions are made with consideration for learning objectives, licensing limitations and operational costs.
