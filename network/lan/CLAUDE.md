# Project: Cisco LAN Architecture & Automation

## 1. Context
- **Purpose**: Design, implement, and automate Cisco campus LAN infrastructure.
- **Focus**: Hierarchical design, VLANs, STP, FHRPs, and Cisco DNA Center integration.

## 2. Core Commands
- **Configuration**: `configure terminal`, `interface ...`, `vlan ...`, `spanning-tree ...`.
- **Verification**: `show vlan brief`, `show spanning-tree summary`, `show ip interface brief`.
- **Automation**: `ansible-playbook campus.yml`, `python scripts/provision_vlans.py`.

## 3. LAN Engineering Standards
- **Design**: Adhere to Cisco's 3-tier or collapsed core hierarchy.
- **Redundancy**: Implement STP, HSRP/GLBP/VRRP for link and device resiliency.
- **Security**: Use port security, DHCP snooping, and dynamic ARP inspection (DAI).

## 4. Workflows
- **Discovery**: Review network diagrams and current switch configurations.
- **Automation Scripting**: Develop playbooks for VLAN deployment and port configuration.
- **Deployment**: Test configurations in a lab environment before production.

## 5. Anti-Patterns
- NO manual configuration changes for routine tasks.
- NO STP loops; ensure proper root bridge election and convergence.
- NO insecure port configurations (e.g., unused ports enabled).

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
