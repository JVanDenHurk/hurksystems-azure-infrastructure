# 01 – Subscription and Cost Management

## Overview

The initial phase of the HurkSystems Azure infrastructure project establishes the Azure subscription and implements cost management controls before deploying cloud resources.

## Objective

Establish a dedicated sandbox subscription and configure financial monitoring to minimise the risk of unexpected Azure charges.

## Subscription Configuration

| Setting | Configuration |
|---|---|
| Subscription name | sub-hurksystems-sandbox |
| Subscription type | Pay-As-You-Go |
| Environment | Sandbox |
| Billing agreement | Microsoft Customer Agreement |

## Naming Convention

The following naming convention has been adopted for Azure subscriptions:

`sub-<organisation>-<environment>`

This provides consistent resource identification and distinguishes subscriptions according to their purpose.

## Budget Configuration

| Setting | Configuration |
|---|---|
| Budget name | budget-hurksystems-sandbox |
| Scope | Billing profile |
| Budget amount | $1.00 |
| Reset period | Monthly |
| Alert type | Actual cost |
| Alert thresholds | 1%, 50%, 80%, 100% |
| Notification method | Email |

## Design Decisions

A Pay-As-You-Go subscription was selected to provide access to Azure services without committing to a fixed monthly expenditure.

A low monthly budget was established to provide early notification of unexpected resource consumption.

The budget was configured at the billing profile scope to align with the local billing currency.

Instance numbers were omitted from subscription and budget names because multiple instances are not currently required.

## Validation

- Azure subscription created successfully.
- Subscription naming convention established.
- Monthly budget configured.
- Cost alert thresholds configured.
- Email notification recipient configured.
- Evaluated spend confirmed at $0.00.
- Billing profile budget currency pending final verification.

## Cost Considerations

Azure budgets provide expenditure notifications but do not enforce a hard spending limit.

Budget notifications may be delayed due to Azure cost processing. Additional preventative controls will be implemented using Azure Policy.

## Outcome

The initial Azure subscription and cost monitoring foundation has been established. The environment is ready for tenant configuration and identity management.

## References

- [Azure resource naming conventions](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/resource-naming)
- [Create and manage Azure budgets](https://learn.microsoft.com/en-us/azure/cost-management-billing/costs/tutorial-acm-create-budgets)