# undefined

**Summary**: One sentence describing this note.
**Tags**: #topic1 #topic2
**Created**: 2026-04-06T00:00:00+00:00
**Last Updated**: 2026-04-06T00:00:00+00:00

---

## Content

Write the main content here.

## Related Notes

- [[Note Title]]

# Project: Cisco Enterprise Network

## 1. Context
- **Purpose**: Design, implement, and automate Cisco enterprise network infrastructure.
- **Focus**: LAN, WAN, wireless, and network security using Cisco technologies.

## 2. Core Commands
- **IOS XE CLI**: `show running-config`, `show interfaces`, `show ip route`.
- **WLC CLI**: `show ap summary`, `show wifi-client`, `show controllers`.
- **Automation**: `python scripts/deploy_config.py`, `ansible-playbook network_config.yml`.
- **Verification**: `ping`, `traceroute`, `show cdp neighbors`.

## 3. Network Engineering Standards
- **Architecture**: Follow Cisco enterprise design patterns (hierarchical, modular).
- **High Availability**: Implement redundancy with HSRP, VSS, StackWise, or vPC.
- **Security**: Apply defense-in-depth with ACLs, port security, and segmentation.
- **Automation**: Script repetitive tasks using Python and Ansible.

## 4. Workflows
- **Discovery**: Review existing network topology and documentation.
- **Planning**: Design addressing, VLANs, and routing before configuration.
- **Automation**: Develop scripts for consistent, repeatable deployments.
- **Verification**: Test changes in lab before production rollout.

## 5. Anti-Patterns
- NO single points of failure in critical network paths.
- NO hardcoded credentials in automation scripts.
- NO unchecked configuration changes without rollback plans.
- NO unmanaged growth of VLANs or IP addressing schemes.

## 6. Logs & Git
- **Git Operations:** Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Conversations:** Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
- **Commit Format:** Follow Conventional Commits.
