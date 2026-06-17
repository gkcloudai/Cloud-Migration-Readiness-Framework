# Go / No-Go Checklist

Run this gate before any production cutover. A single No on a critical-path item is a No-Go unless explicitly waived by the Accountable owner with a documented mitigation.

## 1. Readiness
- [ ] All critical-path components marked Ready in the readiness tracker
- [ ] No open Blocked items on the critical path
- [ ] Terraform for critical-path components at Production maturity

## 2. Approvals
- [ ] Security and IAM sign-off recorded
- [ ] Change-management ticket approved
- [ ] Data owner sign-off for any data migration

## 3. Resilience
- [ ] Rollback plan documented and tested
- [ ] DR / failover validated (game-day completed)
- [ ] Backups verified and restore tested within RPO

## 4. Operations
- [ ] Observability dashboards and alerts live for the new path
- [ ] On-call coverage confirmed for cutover window plus 48 hours
- [ ] Runbook published and linked

## 5. Communication
- [ ] Cutover window communicated to stakeholders
- [ ] Status channel and escalation path defined
- [ ] Customer / downstream impact assessed and communicated

## Decision
- [ ] **GO** - all critical items pass
- [ ] **NO-GO** - one or more critical items fail; reschedule and re-gate

Decision owner: ______________  Date: __________  Mitigations / waivers: ______________
