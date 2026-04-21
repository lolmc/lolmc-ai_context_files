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

# Project: Cisco WAN Engineering & Automation

## 1. Context
- **Purpose**: Design, implement, and automate Cisco WAN infrastructure.
- **Focus**: SD-WAN, MPLS, QoS, and WAN security.

## 2. Core Commands
- **SD-WAN Config**: `vmanage-cli configure template`, `vsmart-cli apply policy`.
- **Traditional WAN**: `configure terminal` (on routers), `show ip route`, `show policy-map interface`.
- **Automation**: `ansible-playbook site.yml`, `python scripts/deploy_wan.py`.
- **Verification**: `ping`, `traceroute`, `show sdwan monitor ...`.

## 3. WAN Engineering Standards
- **SD-WAN**: Follow Cisco's Enterprise WAN CVDs. Use Application-Aware Routing (AAR).
- **QoS**: Implement Cisco's 8-class or 12-class QoS model end-to-end.
- **Security**: Integrate with Cisco Umbrella/SASE. Use DTLS for vManage communication.

## 4. Workflows
- **Discovery**: Analyze current WAN topology and traffic patterns.
- **Automation Scripting**: Develop modular Ansible roles or Python scripts.
- **Deployment**: Test changes in a lab environment before production.

## 5. Anti-Patterns
- NO manual configuration changes in production.
- NO un-tested QoS policies.
- NO hardcoded credentials in automation scripts.

## 6. Logs & Git
- **Git Operations:** Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Conversations:** Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
- **Commit Format:** Follow Conventional Commits.
