# AZ-104 Lab 02a – Manage Subscriptions and RBAC

## Objective
Understand Azure governance using management groups and role-based access control (RBAC).

## Concepts Covered
- Management groups and hierarchy
- Azure RBAC fundamentals
- Built-in vs custom roles
- Scope and inheritance
- Activity Log auditing

## What I Practiced
- Created a management group
- Assigned built-in roles at management group scope
- Created a custom RBAC role using least privilege
- Verified role creation using Activity Log

## Key Learnings
- Management groups enable governance across subscriptions
- RBAC is based on principal, role, and scope
- Custom roles help enforce least privilege
- Permissions assigned at higher scope are inherited

## Interview Notes
Management groups sit above subscriptions.  
RBAC roles control access to Azure resources.  
Custom roles are defined using Actions, NotActions, and AssignableScopes.
