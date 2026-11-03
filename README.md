# AI Cloud Security Lab: Vulnerable & Defended Document Assistant

## Project Overview
This repository documents a 16-week lab that will build practical security implementation demonstrating real-world cloud security, agentic AI trust boundaries, and IAM least privilege in AWS. 

The lab centers around an intentionally constrained multi-tenant financial document assistant (synthetic settlement records) built with Amazon Bedrock, AWS Lambda, and Terraform. The objective is to construct an intentionally vulnerable system, demonstrate five bounded adversarial attack vectors (e.g., prompt injection, broken tenant isolation, unauthorized tool invocation), and implement defense-in-depth mitigations backed by automated regression tests and incident runbooks.

## Project Structure
ai-cloud-security-lab/
├── README.md
├── .gitignore
├── docs/
│   ├── scope.md
│   ├── architecture.md
│   ├── data-classification.md
│   ├── inventory.md
│   ├── cost-log.md
│   └── incidents/
│       └── capital-one-2019.md
├── infrastructure/
│   └── README.md
├── app/
│   └── README.md
├── data/
│   └── README.md
└── tests/
└── README.md

## Current Status (Week 1)
- **Phase:** Phase 1 — Foundation and Account Security
- **Milestone:** Threat Model & Lab Account Setup
- **Current Deliverables:**
  - Dedicated personal AWS lab account configured with MFA and spending alerts.
  - Initial repository layout and threat modeling documentation established.
  - Data classification matrix drafted for synthetic multi-tenant records.
  - Initial cloud threat analysis completed for the 2019 Capital One SSRF breach.

## Phase Roadmap
- **Weeks 1–6 (Project 1):** Terraform baseline, policy testing, logging, and account-level threat modeling.
- **Weeks 7–11 (Project 2):** Bedrock Agent implementation, synthetic multi-tenant corpus, and 5 bounded attack demonstrations.
- **Weeks 12–15 (Project 3):** Dual-layer authorization, content filtering/guardrails, monitoring, and incident response runbooks.
- **Week 16 (Career Launch):** Portfolio walkthrough and security interview scenario rehearsal.