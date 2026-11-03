# Infrastructure Cost & Resource Log

*Operating Principle: Budgets generate notifications but do not halt billing. All non-persistent infrastructure must be tracked and destroyed after testing sessions.*

| Date | Service / Resource | Purpose | Estimated Monthly Cost | Actual Billed Amount | Decommissioned? |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 2026-10-03 | AWS Budgets (1 Budget) | Spend alert threshold monitoring ($10 cap) | $0.00 (First 2 budgets free) | $0.00 | No (Persistent) |
| 2026-10-03 | IAM / IAM Identity Center | Administrative identity & MFA configuration | $0.00 (Native feature) | $0.00 | No (Persistent) |
| Planned | S3 Bucket (Documents) | Synthetic settlement document corpus storage | TBD | TBD | Post-session teardown |
| Planned | AWS Lambda | Action group tool execution | Free Tier / < $0.10 | TBD | Managed via Terraform |
| Planned | Amazon Bedrock (Inference) | Foundation model test invocations | TBD | TBD | On-demand usage |