# Arkadiy Ayrapetov

Network and OT security engineer, 13+ years building and defending enterprise and industrial networks. This is where I publish small, read-only tools and notes from what I've learned along the way.

**Focus areas**
- Network access control: Cisco ISE, TrustSec / SGT, 802.1X, EAP-TLS, TEAP, RADIUS and TACACS+
- Campus fabric: Catalyst Center, SD-Access, LISP / VXLAN
- OT / ICS security: segmentation, Purdue model, IEC 62443 and NIST 800-82
- Network detection and monitoring: NetFlow, Secure Network Analytics, NDR platforms
- Automation: Python, Netmiko, PowerShell, read-only by default

**Certifications:** Cisco CCNP Enterprise · CompTIA CySA+, CSAP, Security+

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

Security reports for any project: see its SECURITY.md.