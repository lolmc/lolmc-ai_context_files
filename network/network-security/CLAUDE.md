# Project: Cisco Wireless Security Best Practices

## 1. Context
- **Purpose**: Secure Cisco wireless networks and services.
- **Focus**: WPA3-Enterprise, 802.1X, guest access, rogue AP detection.

## 2. Core Commands
- **WLC Config**: `configure wireless controller`, `security wpa akg ...`, `security dot1x ...`.
- **ISE Integration**: `radius server ...` (pointing to ISE), `network access policy ...`.
- **Verification**: `show wlan id <id>`, `show ap auth-list`, `show wireless client`.

## 3. Wireless Security Standards
- **Authentication**: Mandate WPA3-Enterprise with EAP-TLS or PEAP.
- **Guest Network**: Isolate guest traffic; use captive portals and bandwidth throttling.
- **Segmentation**: Use VLANs and policies to separate corporate, guest, and IoT traffic.
- **Rogue APs**: Enable detection and mitigation features on WLCs and ISE.

## 4. Workflows
- **Discovery**: Review current wireless SSIDs and security configurations.
- **Policy Implementation**: Configure WLCs and ISE for secure authentication.
- **Validation**: Test client connectivity and security posture.

## 5. Anti-Patterns
- NO WPA2-PSK for corporate networks.
- NO open guest SSIDs without captive portals.
- NO unmonitored rogue AP alerts.

## 6. Logs & Git
- **Conversations**: Mandatory record of all interactions in `CONVERSATIONS.log`.
- **Commit Format**: Follow Conventional Commits.
