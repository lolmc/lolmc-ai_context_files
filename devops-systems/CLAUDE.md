# Project: DevOps & Systems Infrastructure

## 1. Context
- **Purpose**: Infrastructure as Code (IaC), CI/CD pipelines, and systems automation.
- **Goal**: Ensure reliable, repeatable, and secure deployments.

## 2. Core Commands
- **Install/Init**: `terraform init`, `docker build`.
- **Validation**: `terraform plan`, `shellcheck scripts/*.sh`.
- **Apply**: `terraform apply`.
- **Scan**: `trivy image [name]`.

## 3. Coding Standards (IaC & Shell)
- **Shell**: Use `sh` or `bash` with strict error handling (`set -euo pipefail`).
- **Docker**: No root users, multi-stage builds, minimal base images.
- **CI/CD**: modular actions/templates for reusability.

## 4. Workflows
- **Discovery**: Read Dockerfiles and CI/CD config files before modification.
- **Safety**: Perform dry-runs or plans before applying changes.
- **Verification**: Verify service health post-deployment.

## 5. Anti-Patterns
- NO hardcoded secrets or .env files in the repository.
- NO unverified shell scripts.
- NO manual production changes; everything via IaC.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
