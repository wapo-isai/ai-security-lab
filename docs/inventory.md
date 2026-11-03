# Environment Inventory

## Current State (Week 1 Baseline)

| Category | Component / Setting | Current Configuration | Status |
| :--- | :--- | :--- | :--- |
| **AWS Account** | Account ID / Dedicated Sandbox | Personal AWS Account (Single-Region: `us-east-1`) | Active |
| **Root Access** | Account Root User | Hardware/FIDO2 or Virtual MFA enabled; zero active access keys | Secured |
| **Administrative Access** | IAM Identity Center / Admin Role | Named administrator principal with MFA; zero long-term root usage | Active |
| **Cost Control** | AWS Budgets | $10.00 USD monthly budget with 50%, 80%, and 100% email threshold alerts | Active |
| **Source Control** | Git Repository | Local/Private repository with `.gitignore` enforcing secret/state exclusion | Active |

## Planned Resources (Weeks 2–15)

| Planned Component | Planned Service | Purpose |
| :--- | :--- | :--- |
| **Base Infrastructure** | HashiCorp Terraform | Reproducible deployment of all lab roles, policies, and buckets |
| **Audit Logging** | AWS CloudTrail & CloudWatch Logs | Capturing management and data-plane API actions across the account |
| **AI Orchestration** | Amazon Bedrock (Agent / Converse) | Document retrieval, tool decision-making, and user interaction |
| **Tool Execution** | AWS Lambda | Action group execution role validating parameters and running export tasks |
| **Corpus Storage** | Amazon S3 + Vector Store / Bedrock KB | Storage of synthetic Tenant A and Tenant B settlement files |
| **Application Layer** | Amazon API Gateway / Python Service | Authenticating incoming analyst requests and passing claims |