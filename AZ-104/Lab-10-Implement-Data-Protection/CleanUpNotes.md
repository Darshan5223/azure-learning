# Lab 10 Cleanup Notes

## Issue
Unable to delete Recovery Services Vault and resource group.

## Reason
Azure Backup uses Soft Delete (14 days) to protect backup data.

## Observations
- VM backup stopped successfully
- Backup data retained due to soft delete
- Restore point collections cannot be deleted manually

## Resolution
Wait for retention period OR disable soft delete (only if allowed).

## Learning
Azure intentionally blocks deletion to protect against data loss and ransomware.
