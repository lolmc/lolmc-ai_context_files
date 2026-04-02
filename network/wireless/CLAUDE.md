# Project: Cisco Wireless Network Design & Automation

## 1. Context
- **Purpose**: Design, implement, and automate Cisco wireless networks.
- **Focus**: WLC configuration, RF design, SSID management, and wireless security.

## 2. Core Commands
- **WLC CLI**: `show ap summary`, `show wifi-client`, `show controllers`.
- **Configuration**: `configure terminal` (on WLCs), `wireless` commands.
- **Automation**: `python scripts/deploy_ssids.py`, `ansible-playbook wlc_config.yml`.
- **RF Tools**: `ekahau`, `airmagnet` (for site surveys).

## 3. Wireless Engineering Standards
- **RF Design**: Optimize for Wi-Fi 6/6E, use RRM for channel/power, CleanAir for interference.
- **Security**: Implement WPA3-Enterprise, 802.1X, and integrate with Cisco ISE.
- **High Density**: Design for 5GHz/6GHz bands, consider micro-cell designs.

## 4. Workflows
- **Discovery**: Review site surveys and existing wireless configurations.
- **Automation Scripting**: Develop scripts for SSID deployment and WLC parameter tuning.
- **Deployment**: Test new configurations in a lab before rolling out.

## 5. Anti-Patterns
- NO manual WLC configuration for mass changes.
- NO poor RF planning leading to coverage gaps or interference.
- NO insecure wireless configurations (e.g., WPA2-PSK for corporate).

## 6. Logs & Git
- **Git Operations:** Always perform `git add`, `git commit`, and `git push` after completing a file edit.
- **Conversations:** Always log conversations between the user and the agent in a file called `CONVERSATIONS.log`.
- **Commit Format:** Follow Conventional Commits.

