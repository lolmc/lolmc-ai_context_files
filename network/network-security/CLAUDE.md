# Project: Cisco Firepower Management Center (FMC)

## 1. Context
- **Purpose**: Centralized management of Cisco Firepower Threat Defense (FTD) devices.
- **Focus**: Policy creation, threat detection, device management, and reporting.

## 2. Core Commands
- **FMC API**: Use `nfv-tools` or direct REST API calls for automation.
- **Policy Management**: `configure access-policy`, `configure intrusion-policy`.
- **Device Management**: `device-group`, `add device`.
- **Monitoring**: `show security intelligence`, `show intrusion event details`.

## 3. FMC Best Practices
- **Policy Design**: Implement access rules based on least privilege; use security intelligence feeds.
- **Intrusion Prevention**: Tune IPS policies for network-specific threats; monitor intrusion events.
- **AMP/URL Filtering**: Configure and regularly update AMP and URL filtering policies.
- **Updates**: Keep FMC and FTD software updated with the latest security patches.

## 4. Workflows
- **Discovery**: Review existing security policies and device configurations.
- **Policy Tuning**: Regularly analyze security events to refine policies.
- **Reporting**: Generate regular reports on threat activity and network security posture.

## 5. Anti-Patterns
- NO broad or overly permissive security policies.
- NO neglecting regular policy tuning or threat analysis.
- NO unpatched FMC or FTD devices.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
