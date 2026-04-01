# Project: Cisco Catalyst Center Automation

## 1. Context
- **Purpose**: Automate network provisioning, assurance, and management using Cisco Catalyst Center.
- **Focus**: REST APIs, SDKs, intent-based workflows, and SD-Access fabric automation.

## 2. Core Commands
- **Catalyst Center API**: `dnacentersdk` Python library usage.
- **Provisioning**: `create_site`, `onboard_device`, `deploy_fabric`.
- **Assurance**: `get_network_health`, `search_device_issues`.
- **Compliance**: `get_config_compliance_status`.

## 3. Catalyst Center Standards
- **IBN**: Translate business intent into network configurations.
- **API Usage**: Use idempotency where possible; handle API errors gracefully.
- **Modularity**: Structure automation scripts for reusability.
- **Security**: Securely manage Catalyst Center API credentials.

## 4. Workflows
- **Discovery**: Understand Catalyst Center topology and existing configurations.
- **Automation Scripting**: Develop scripts for common provisioning tasks.
- **Testing**: Test automation scripts in a lab environment before production.

## 5. Anti-Patterns
- NO direct CLI access for configuration when automation is possible.
- NO un-secured API credentials.
- NO manual changes to automated configurations.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
