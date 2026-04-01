# Project: Cisco ASA Firewall Configuration

## 1. Context
- **Purpose**: Secure network perimeters using Cisco ASA firewalls.
- **Focus**: Stateful inspection, NAT, VPN, access control, and threat prevention.

## 2. Core Commands
- **Configuration**: `configure terminal`, `access-list ...`, `nat ...`, `crypto ipsec ...`.
- **Verification**: `show run http`, `show xlate`, `show crypto ipsec sa`, `show threat-detection statistics`.
- **Monitoring**: `show log`, `show conn`.

## 3. ASA Firewall Standards
- **Policy Design**: Implement rules with least privilege; deny by default.
- **NAT**: Use object NAT for clarity and maintainability.
- **VPN**: Utilize strong encryption (AES-GCM) and authentication (IKEv2).
- **Threat Defense**: Enable and tune IPS/IDS policies.

## 4. Workflows
- **Discovery**: Review existing ASA policy and network topology.
- **Implementation**: Test configuration changes in a lab before production.
- **Verification**: Validate policy effectiveness and monitor for threats.

## 5. Anti-Patterns
- NO any/permit any rules in critical security zones.
- NO use of weak encryption or authentication for VPNs.
- NO un-monitored firewall logs.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
