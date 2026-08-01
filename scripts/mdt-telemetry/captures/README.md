# Telemetry Capture Data

Sample MDT telemetry data captured from two Catalyst 9300 switches (`cat9300x-pod10a` / `cat9300-pod10b`) running IOS XE 26.01.1. Captured using the OTel collector in capture mode over a 120-second window.

**55 of 66 subscriptions produced data.** 10 were silent (features not configured on these switches).

## File Index

Each file is named `<sub-id>-<yang-module-slug>.txt` and contains grouped plain-text metric summaries.

### HOT Tier (30s) — 4 files

| Sub | § | Feature | File | Data Points |
|-----|---|---------|------|-------------|
| 30001 | 1 | CPU Utilization | `30001-cisco-ios-xe-process-cpu-oper_cpu-usage_cpu-utilization.txt` | 60,700 |
| 30002 | 3 | Process Memory | `30002-cisco-ios-xe-process-memory-oper_memory-usage-processes_memo.txt` | 53,920 |
| 30003 | 7 | Interface Statistics | `30003-cisco-ios-xe-interfaces-oper_interfaces_interface.txt` | 79,950 |
| 30004 | 44 | Punt/Inject Counters | `30004-cisco-ios-xe-switch-dp-punt-inject-oper_switch-dp-punt-injec.txt` | 4,160 |

### WARM Tier (60s) — 22 files (7 silent)

| Sub | § | Feature | File | Data Points |
|-----|---|---------|------|-------------|
| 60001 | 2 | Memory Statistics | `60001-cisco-ios-xe-memory-oper_memory-statistics_memory-statistic.txt` | 108 |
| 60002 | 4 | System DRAM | `60002-cisco-ios-xe-platform-software-oper_cisco-platform-software_.txt` | 888 |
| 60003 | 5 | Environment Sensors | `60003-cisco-ios-xe-environment-oper_environment-sensors.txt` | 606 |
| 60004 | 6 | PoE Operational | `60004-cisco-ios-xe-poe-oper_poe-oper-data.txt` | 1,020 |
| 60005 | 8 | Spanning Tree | `60005-cisco-ios-xe-spanning-tree-oper_stp-details.txt` | 2,748 |
| 60006 | 9 | Stack Health | `60006-cisco-ios-xe-stack-oper_stack-oper-data.txt` | 288 |
| 60007 | 15 | Platform Components | `60007-cisco-ios-xe-platform-oper_components_component.txt` | 10,650 |
| 60008 | 24 | BGP State | `60008-cisco-ios-xe-bgp-oper_bgp-state-data.txt` | 2,142 |
| 60009 | 25 | OSPF State | `60009-cisco-ios-xe-ospf-oper_ospf-oper-data.txt` | 1,368 |
| 60010 | 33 | NTP Synchronization | `60010-cisco-ios-xe-ntp-oper_ntp-oper-data_ntp-status-info.txt` | 156 |
| 60011 | 34 | BFD Sessions | `60011-cisco-ios-xe-bfd-oper_bfd-state_sessions_session.txt` | 108 |
| 60012 | 35 | HSRP State | `60012-cisco-ios-xe-hsrp-oper_hsrp-oper-data_hsrp-group-info.txt` | 42 |
| 60013 | 36 | VRRP State | `60013-cisco-ios-xe-vrrp-oper_vrrp-oper-data_vrrp-oper-state.txt` | 192 |
| 60014 | 37 | Flow Monitor | `60014-cisco-ios-xe-flow-monitor-oper_flow-monitors_flow-monitor.txt` | 6 |
| 60015 | 38 | IP SLA Probes | `60015-cisco-ios-xe-ip-sla-oper_ip-sla-stats_sla-oper-entry.txt` | 96 |
| 60016 | 46 | CEF / FIB State | `60016-cisco-ios-xe-fib-oper_fib-oper-data.txt` | 30,480 |
| 60017 | 49 | BGP Neighbor Detail | `60017-cisco-ios-xe-bgp-nbr-oper_bgp-nbr-oper-data.txt` | 378 |
| 60018 | 53 | IS-IS Interface | `60018-cisco-ios-xe-isis-intf-oper_isis-intf-oper-data_isis-if-tag-.txt` | 210 |
| 60019 | 54 | Multicast Routing | `60019-cisco-ios-xe-mroute-oper_mroute-oper-data_mroute-state.txt` | 171 |
| 60020 | 55 | Stack Member | `60020-cisco-ios-xe-stack-member-oper_stack-member-oper-data_locati.txt` | 282 |
| 60021 | 56 | Tunnel Interface | `60021-cisco-ios-xe-tunnel-oper_tunnel-oper-data_tunnel-if.txt` | 210 |
| 60022 | 59 | PIM Multicast | `60022-cisco-ios-xe-pim-oper_pim-oper-data.txt` | 33 |
| 60027 | 67 | IETF Interfaces | `60027-ietf-interfaces_interfaces-state_interface.txt` | 10,242 |
| 60028 | 26 | IETF Routing State | `60028-ietf-routing_routing-state_routing-instance.txt` | 1,176 |

### COOL Tier (300s) — 29 files (4 silent)

| Sub | § | Feature | File | Data Points |
|-----|---|---------|------|-------------|
| 50001 | 10 | VLANs | `50001-cisco-ios-xe-vlan-oper_vlans_vlan.txt` | 214 |
| 50002 | 11 | MAC Address Table | `50002-cisco-ios-xe-matm-oper_matm-oper-data_matm-table.txt` | 461 |
| 50003 | 12 | ARP Table | `50003-cisco-ios-xe-arp-oper_arp-data_arp-vrf.txt` | 260 |
| 50004 | 13 | LLDP Neighbors | `50004-cisco-ios-xe-lldp-oper_lldp-entries.txt` | 585 |
| 50005 | 14 | CDP Neighbors | `50005-cisco-ios-xe-cdp-oper_cdp-neighbor-details_cdp-neighbor-deta.txt` | 155 |
| 50006 | 16 | Device Hardware | `50006-cisco-ios-xe-device-hardware-oper_device-hardware-data_devic.txt` | 250 |
| 50007 | 17 | Switchport | `50007-cisco-ios-xe-switchport-oper_switchport-oper-data_switchport.txt` | 1,261 |
| 50010 | 20 | 802.1X / Identity | `50010-cisco-ios-xe-identity-oper_identity-oper-data.txt` | 186 |
| 50011 | 21 | TCAM Utilization | `50011-cisco-ios-xe-tcam-oper_tcam-details_tcam-detail.txt` | 312 |
| 50012 | 22 | MDT Health | `50012-cisco-ios-xe-mdt-oper-v2_mdt-oper-v2-data.txt` | 2,323 |
| 50013 | 23 | Software Install | `50013-cisco-ios-xe-install-oper_install-oper-data.txt` | 1,113 |
| 50014 | 27 | DHCP | `50014-cisco-ios-xe-dhcp-oper_dhcp-oper-data.txt` | 28 |
| 50015 | 28 | HA State | `50015-cisco-ios-xe-ha-oper_ha-oper-data_ha-infra.txt` | 20 |
| 50017 | 30 | TrustSec | `50017-cisco-ios-xe-trustsec-oper_trustsec-state.txt` | 12 |
| 50019 | 32 | ACL Counters | `50019-cisco-ios-xe-acl-oper_access-lists_access-list.txt` | 276 |
| 50020 | 39 | AAA / RADIUS | `50020-cisco-ios-xe-aaa-oper_aaa-data_aaa-radius-stats.txt` | 156 |
| 50021 | 40 | Port Security | `50021-cisco-ios-xe-psecure-oper_psecure-oper-data_psecure-state.txt` | 16 |
| 50022 | 41a | MACsec | `50022-cisco-ios-xe-macsec-oper_macsec-oper-data_macsec-statistics.txt` | 828 |
| 50023 | 41b | MKA | `50023-cisco-ios-xe-mka-oper_mka-oper-data_mka-statistics.txt` | 350 |
| 50024 | 42 | VRF | `50024-cisco-ios-xe-vrf-oper_vrf-oper-data_vrf-entry.txt` | 8 |
| 50025 | 43 | DP Resources | `50025-cisco-ios-xe-switch-dp-resources-oper_switch-dp-resources-op.txt` | 3,668 |
| 50026 | 47 | EIGRP | `50026-cisco-ios-xe-eigrp-oper_eigrp-oper-data_eigrp-instance.txt` | 474 |
| 50027 | 48 | IS-IS | `50027-cisco-ios-xe-isis-oper_isis-oper-data_isis-instance.txt` | 14 |
| 50028 | 50 | BGP RIB Detail | `50028-cisco-ios-xe-bgp-rib-oper_bgp-rib-oper-data_bgp-route.txt` | 24 |
| 50029 | 51 | High-Scale ARP | `50029-cisco-ios-xe-ip-arp-oper_ip-arp-oper-data_ni-ip-arp_ip-arp-e.txt` | 144 |
| 50030 | 52 | IPv6 ND | `50030-cisco-ios-xe-ipv6-nd-oper_ipv6-nd-oper-data_ni-ipv6-nd_ipv6-.txt` | 56 |
| 50031 | 57 | YANG Interfaces | `50031-cisco-ios-xe-yang-interfaces-oper_yang-interfaces-oper-data.txt` | 50 |

### Silent Subscriptions (no capture file — feature not configured)

| Sub | § | Feature | Reason |
|-----|---|---------|--------|
| 50008 | 18 | Transceiver / Optics | No SFP modules installed |
| 50009 | 19 | UDLD | UDLD not enabled |
| 50016 | 29 | Linecard Status | Fixed-form-factor chassis |
| 50018 | 31 | LACP / Port-Channel | No port-channels configured |
| 50032 | 61 | MPLS Forwarding | MPLS not enabled |
| 50033 | 65 | PTP / SyncE Timing | No PTP hardware |
| 60023 | 60 | MPLS LDP | MPLS not enabled |
| 60024 | 62 | LISP | LISP not configured |
| 60025 | 63 | VXLAN NVE | VXLAN not configured |
| 60026 | 64 | EVPN | EVPN not configured |

## Usage

- **Dashboard development**: Use as authoritative field-name source — each file shows exact `cisco.content.*` metric names and dimensions
- **Validation**: Cross-reference KPI tables against actual leaf paths in captured data
- **Sample data for Splunk**: Convert to JSONL for Splunk test ingestion
