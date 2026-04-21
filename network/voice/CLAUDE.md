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

# Project: Cisco Voice & Collaboration Systems

## 1. Context
- **Purpose**: Deploying and managing Cisco Unified Communications Manager (CUCM) and related services.
- **Focus**: Dial plans, QoS, security, and collaboration endpoints.

## 2. Core Commands
- **CUCM CLI**: `utils os select-version ...`, `utils network capture ...`.
- **AXL API**: `udt_cli` or Python scripts using `zeep` for user provisioning.
- **Verification**: `show isdn status`, `show sip-ua connections`, `show ccsip summary`.
- **QoS CLI**: `mls qos` on switches, `policy-map` on routers.

## 3. Voice Engineering Standards
- **Dial Plan**: Implement a scalable and logical dial plan for internal and external calls.
- **QoS**: Prioritize voice traffic using EF marking and appropriate queuing.
- **Security**: Ensure SRTP and TLS are enabled for sensitive calls.

## 4. Workflows
- **Discovery**: Review current CUCM cluster configuration and dial plan.
- **User Provisioning**: Automate user creation and endpoint assignment via AXL.
- **Troubleshooting**: Use call tracing tools and logs to diagnose issues.

## 5. Anti-Patterns
- NO un-documented dial plan changes.
- NO insecure voice protocols (e.g., unencrypted SIP).
- NO manual user management for large deployments.

## 6. Logs & Git
- **Git Operations:** Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Conversations:** Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
- **Commit Format:** Follow Conventional Commits.
