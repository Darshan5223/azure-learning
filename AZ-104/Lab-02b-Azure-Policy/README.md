# AZ-104 Lab 02b – Administer Governance via Azure Policy

## Objective
Understand how Azure Policy, tags, and resource locks are used to enforce governance and compliance across Azure resources.

## Lab Scenario
The organization identified resources without ownership, cost center, or project information.
This lab focuses on enforcing tagging standards, remediating existing resources, and protecting
critical resources using governance controls.

## Concepts Covered
- Azure Policy fundamentals
- Policy definitions and assignments
- Policy effects (Deny, Audit, Modify, DeployIfNotExists)
- Policy scope and inheritance
- Remediation tasks and managed identity
- Azure tags and tagging strategy
- Resource locks (Delete vs ReadOnly)
- Azure Policy vs Azure RBAC

## What I Practiced
- Created and applied tags at the resource group level
- Enforced mandatory tags using Azure Policy (Deny effect)
- Remediated non-compliant resources using Modify policy
- Used remediation tasks with managed identity
- Verified compliance through policy evaluation
- Protected resources using delete locks

## Key Learnings
- Azure Policy enforces organizational standards, RBAC controls permissions
- Deny policies block non-compliant deployments
- Modify policies automatically remediate existing resources
- Remediation tasks are required for existing resources
- Resource locks override RBAC permissions
- Governance combines Policy, RBAC, and Locks

## Real-World Use Case
- Enforcing cost center and ownership tagging
- Preventing non-compliant deployments
- Automatically fixing governance drift
- Protecting production resources from accidental deletion

## Interview Notes
- Azure Policy is a pre-deployment security and compliance tool
- RBAC controls who can do what on Azure resources
- Remediation tasks fix existing non-compliant resources
- Assigning policy at higher scope ensures inheritance
- Resource locks override RBAC permissions

## Documentation
Refer to the attached PDF for detailed explanations, commands, and interview-ready Q&A.
