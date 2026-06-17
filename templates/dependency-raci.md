# Dependency RACI

Responsibility matrix for a cloud migration program. R = Responsible, A = Accountable, C = Consulted, I = Informed.
Example mapping; adapt roles and workstreams to your org.

| Workstream | Program TPM | Platform Eng | Security / IAM | Data Eng | App Teams | Finance |
|---|---|---|---|---|---|---|
| Readiness tracking | A/R | C | C | C | C | I |
| Networking and VPC | A | R | C | I | I | I |
| GKE cluster provisioning | A | R | C | I | I | I |
| Secrets and KMS policy | A | C | R | C | I | I |
| Data replication / cutover | A | C | C | R | C | I |
| Observability and alerting | A | R | I | C | C | I |
| Application migration | A | C | I | C | R | I |
| Go / No-Go decision | A/R | C | C | C | C | C |
| Cost tracking | A | I | I | I | I | R |
| DR and failover validation | A | R | C | C | I | I |

## How to use

1. One Accountable owner per workstream. Never two.
2. The TPM is Accountable for readiness tracking and the go/no-go decision, not for the engineering work itself.
3. Review the matrix at program kickoff and re-confirm before cutover.
