# Lab Scope and Operating Rules

## Purpose
The purpose of this environment is to analyze, execute, and defend against security vulnerabilities in cloud and agentic AI architectures within a safely isolated, non-production sandbox.

## Target Environment & Boundaries
* **Account Boundary:** All actions, resources, roles, and tests are strictly confined to a single dedicated, personal AWS account (`us-east-1` or designated primary region). No corporate, client, or shared organization infrastructure will ever be targeted or connected.
* **Test Sinks:** All tool execution actions (e.g., simulated document exports, ticket generation, alert notifications) route strictly to private, controlled local sinks (such as local stdout, mock HTTP endpoints, or private test S3 buckets). Outbound external webhooks or untrusted external endpoints are out of scope.
* **Data Boundary:** Only 100% synthetic financial records (settlement and mortgage examples) are generated and stored. No proprietary, customer, or real personally identifiable information (PII) is permitted in prompts, source data, or embeddings.
* **Adversarial Boundaries:** Vulnerability demonstrations are strictly local and application-scoped (e.g., indirect prompt injection, parameter tampering, cross-tenant context leakage). Denial-of-service (DoS) attacks against AWS infrastructure endpoints and attacks targeting the underlying hypervisor or managed AI model weights are explicitly prohibited.