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

# Project: Cisco Firepower Threat Defense (FTD) Configuration

## 1. Context
- **Purpose**: Configure and manage individual Cisco Firepower Threat Defense (FTD) devices.
- **Focus**: Firewall policies, NAT, VPN, IPS, AMP, and URL filtering directly on FTD.

## 2. Core Commands
- **CLI**: `configure terminal`, `access-list ...`, `nat ...`, `crypto ipsec ...`, `policy-map type inspect dns ...`.
- **Verification**: `show run access-list`, `show conn`, `show crypto ipsec sa`, `show policy-map type inspect dns`.
- **Troubleshooting**: `packet-tracer ...`, `capture-data ...`.

## 3. FTD Device Standards
- **Policy Design**: Implement rules based on least privilege; deny by default.
- **NAT**: Use interface NAT or twice NAT as appropriate for the topology.
- **VPN**: Utilize strong encryption (AES-GCM) and authentication (IKEv2) for tunnels.
- **Threat Defense**: Configure and tune IPS/AMP for network-specific threats.

## 4. Workflows
- **Discovery**: Review existing FTD configurations and network requirements.
- **Implementation**: Test configurations in a lab environment before deployment.
- **Verification**: Validate policy effectiveness and monitor threat detection logs.

## 5. Anti-Patterns
- NO overly permissive access rules.
- NO weak encryption for VPNs.
- NO unmonitored threat logs or alerts.

## 6. Logs & Git
- **Git Operations:** Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Conversations:** Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
- **Commit Format:** Follow Conventional Commits.
