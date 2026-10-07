# Arkadiy Ayrapetov

Network and OT security engineer with 13+ years building and defending enterprise and industrial networks. I work as an independent consultant on network access control, segmentation and security monitoring for organizations in public transit, biotech manufacturing and financial services.

**Available for remote consulting engagements.** Contact: [arkadiy@ayrapetov.co](mailto:arkadiy@ayrapetov.co)

**Focus areas**
- Network access control: Cisco ISE, TrustSec / SGT, 802.1X, EAP-TLS, TEAP, RADIUS and TACACS+
- Campus fabric: Catalyst Center, SD-Access, LISP / VXLAN
- OT / ICS security: segmentation, Purdue model, IEC 62443 and NIST 800-82 aligned designs
- Firewalls and VPN: Cisco FTD / FMC, Meraki vMX, Azure networking
- Network detection and monitoring: NetFlow, Secure Network Analytics, NDR platforms
- Automation: Python, Netmiko, PowerShell, read-only by default

**Certifications:** CompTIA CySA+, Security+, CSAP · Cisco CCNP Security, CCNP Enterprise

## What I take on

- **ISE and 802.1X health checks**: certificate, EAP-TLS and TEAP failures, RADIUS failure triage, policy cleanup with backup and rollback
- **TrustSec / SGT segmentation**: design, Monitor-mode rollout, Catalyst Center Group-Based Access Control, enforcement verification
- **Catalyst Center and SD-Access operations**: API automation, Day-N templates that survive reprovisioning, fabric subnet builds
- **Root cause under pressure**: proving or clearing the network with controller history, drop counters and API evidence

## Recent field results

Anonymized results from current engagements:

- Traced a recurring "cannot ping the domain controllers" complaint to a single TrustSec policy cell, proven with hardware drop counters on four fabric edges
- Audited 1,968 switch ports from running-config and cut a planned port-security remediation from 172 ports to the 8 that actually needed it
- Stopped a Catalyst Center resync storm by suppressing link-status traps on about 1,450 host ports through reprovision-safe templates
- Migrated 25 security groups and 9 contracts from ISE to Catalyst Center Group-Based Access Control with zero failures, verified per VRF
- Restored a broken 802.1X EAP-TLS rollout by fixing certificate SAN issuance, then proved TEAP machine-plus-user chaining in a pilot
- Patched a two-node ISE deployment after hours against an actively exploited critical advisory and restored the controller integration the same night

## Open-source tools

| Project | What it does |
|---|---|
| [cisco-interface-health](https://github.com/korpus91/cisco-interface-health) | Offline triage of `show interfaces` output: CRC, duplex mismatch, err-disabled, drops, flapping. `pip install cisco-interface-health` |
| [cisco-config-drift](https://github.com/korpus91/cisco-config-drift) | Read-only baseline vs running-config drift detection for IOS / IOS-XE. `pip install cisco-config-drift` |
| [ise-endpoint-explain](https://github.com/korpus91/ise-endpoint-explain) | Why did this endpoint get what it got: ISE session, auth timeline, authz profile, SGT and failure causes |
| [ise-health-audit](https://github.com/korpus91/ise-health-audit) | Read-only Cisco ISE node health and certificate-expiry audit via the OpenAPI |
| [ios-hardening-audit](https://github.com/korpus91/ios-hardening-audit) | Offline IOS / IOS-XE hardening audit: 23 checks across AAA, credentials, management plane, SNMP, logging. `pip install ios-hardening-audit` |
| [win-security-posture-audit](https://github.com/korpus91/win-security-posture-audit) | Read-only Windows security and health posture audit in PowerShell |

Every tool here is read-only by design: it observes and reports, it never changes a device.

## Writing

Field notes on network and OT security: [korpus91.github.io](https://korpus91.github.io)

## Contact

Security reports for any project: see its SECURITY.md. Consulting inquiries: [arkadiy@ayrapetov.co](mailto:arkadiy@ayrapetov.co)