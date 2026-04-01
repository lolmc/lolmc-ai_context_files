# Project: Cisco Network Device Hardening

## 1. Context
- **Purpose**: Secure Cisco routers and switches against common network threats.
- **Focus**: Access control, service hardening, secure protocols, and logging.

## 2. Core Commands
- **Access**: `ssh vrf <vrf_name>`, `username admin role <role> secret 5 <hash>`.
- **Hardening**: `no service pad`, `no service finger`, `line vty 0 4` (configure transport input ssh).
- **Logging**: `logging buffered 500000 debugging`, `logging host <syslog_server>`.
- **Verification**: `show running-config`, `show ip ssh`, `show snmp user`.

## 3. Hardening Standards
- **AAA**: Implement centralized authentication, authorization, and accounting.
- **Control Plane Policing (CoPP)**: Protect the control plane from excessive traffic.
- **Unused Ports**: Shut down and assign to an unused, non-routable VLAN.
- **Unused Services**: Disable SNMP (unless v3), Telnet, HTTP, etc.

## 4. Workflows
- **Discovery**: Audit existing configurations against hardening benchmarks.
- **Implementation**: Apply hardening configurations systematically.
- **Verification**: Test access and functionality post-hardening.

## 5. Anti-Patterns
- NO Telnet access enabled.
- NO default SNMP community strings.
- NO insecure password storage.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
