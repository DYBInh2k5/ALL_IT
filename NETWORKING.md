# Tổng Hợp Networking & Infrastructure

## 📋 Mục Lục
- [Network Fundamentals](#network-fundamentals)
- [Network Hardware](#network-hardware)
- [Network Protocols](#network-protocols)
- [Network Services](#network-services)
- [Network Security](#network-security)
- [Wireless Networking](#wireless-networking)
- [Network Monitoring](#network-monitoring)
- [Software-Defined Networking](#software-defined-networking)
- [Network Automation](#network-automation)

## 🌐 Network Fundamentals

### OSI Model Layers
| Layer | Name | Function | Examples | Protocols |
|-------|------|----------|----------|-----------|
| **7** | Application | User interface | Web browsers, email | HTTP, SMTP, FTP |
| **6** | Presentation | Data formatting | Encryption, compression | SSL/TLS, JPEG |
| **5** | Session | Session management | Login sessions | NetBIOS, RPC |
| **4** | Transport | End-to-end delivery | Reliable data transfer | TCP, UDP |
| **3** | Network | Routing | Path determination | IP, ICMP, OSPF |
| **2** | Data Link | Frame delivery | Local network delivery | Ethernet, Wi-Fi |
| **1** | Physical | Bit transmission | Electrical signals | Cables, radio waves |

### TCP/IP Model
| Layer | Function | Protocols | Devices |
|-------|----------|-----------|---------|
| **Application** | User services | HTTP, SMTP, DNS, DHCP | Applications |
| **Transport** | Process-to-process | TCP, UDP | Firewalls |
| **Internet** | Host-to-host | IP, ICMP, ARP | Routers |
| **Network Access** | Network interface | Ethernet, Wi-Fi | Switches, NICs |

### IP Addressing
| Type | Format | Range | Use Cases |
|------|--------|-------|-----------|
| **IPv4** | 32-bit dotted decimal | 0.0.0.0 - 255.255.255.255 | Current internet |
| **IPv6** | 128-bit hexadecimal | 2001:db8::1 | Future internet |
| **Private IPv4** | RFC 1918 | 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16 | Internal networks |
| **Link-Local** | Auto-configuration | 169.254.0.0/16 (IPv4), fe80::/10 (IPv6) | Local communication |

### Subnetting
| CIDR | Subnet Mask | Hosts | Use Case |
|------|-------------|-------|----------|
| **/24** | 255.255.255.0 | 254 | Small networks |
| **/16** | 255.255.0.0 | 65,534 | Medium networks |
| **/8** | 255.0.0.0 | 16,777,214 | Large networks |
| **/30** | 255.255.255.252 | 2 | Point-to-point links |

## 🔧 Network Hardware

### Switches
| Type | Features | Use Cases | Examples |
|------|----------|-----------|----------|
| **Unmanaged** | Plug-and-play | Home, small office | Netgear GS108 |
| **Managed** | VLAN, QoS, monitoring | Enterprise | Cisco Catalyst |
| **Layer 3** | Routing capabilities | Inter-VLAN routing | HP Aruba |
| **PoE** | Power over Ethernet | IP phones, cameras | Ubiquiti UniFi |

### Routers
| Type | Features | Use Cases | Examples |
|------|----------|-----------|----------|
| **Home/SOHO** | NAT, Wi-Fi, firewall | Home networks | ASUS, Linksys |
| **Enterprise** | BGP, MPLS, redundancy | Corporate networks | Cisco ISR |
| **Core** | High throughput | Service provider backbone | Juniper MX |
| **Edge** | WAN optimization | Branch offices | Cisco ASR |

### Firewalls
| Type | Capabilities | Deployment | Examples |
|------|-------------|------------|----------|
| **Packet Filter** | Basic filtering | Perimeter | iptables |
| **Stateful** | Connection tracking | Network edge | pfSense |
| **Next-Gen** | Deep packet inspection | Enterprise | Palo Alto |
| **Web Application** | HTTP/HTTPS protection | Web servers | F5, Cloudflare |

### Wireless Access Points
| Type | Standards | Features | Use Cases |
|------|-----------|----------|-----------|
| **Consumer** | Wi-Fi 6/6E | Basic features | Home use |
| **Enterprise** | Wi-Fi 6E/7 | Centralized management | Business |
| **Outdoor** | Weather-resistant | Long range | Campus, public |
| **Mesh** | Self-healing | Easy deployment | Large areas |

## 📡 Network Protocols

### Routing Protocols
| Protocol | Type | Characteristics | Use Cases |
|----------|------|----------------|-----------|
| **RIP** | Distance Vector | Simple, limited | Small networks |
| **OSPF** | Link State | Fast convergence | Enterprise |
| **EIGRP** | Hybrid | Cisco proprietary | Cisco networks |
| **BGP** | Path Vector | Internet routing | ISPs, large enterprises |

### Switching Protocols
| Protocol | Purpose | Features | Implementation |
|----------|---------|----------|----------------|
| **STP** | Loop prevention | Blocking ports | IEEE 802.1D |
| **RSTP** | Rapid convergence | Fast recovery | IEEE 802.1w |
| **VTP** | VLAN management | Centralized config | Cisco proprietary |
| **LACP** | Link aggregation | Bandwidth increase | IEEE 802.3ad |

### Network Services Protocols
| Protocol | Port | Purpose | Security |
|----------|------|---------|---------|
| **DNS** | 53 | Name resolution | DNSSEC |
| **DHCP** | 67/68 | IP assignment | DHCP snooping |
| **NTP** | 123 | Time synchronization | Authentication |
| **SNMP** | 161/162 | Network management | SNMPv3 |

### Application Protocols
| Protocol | Port | Purpose | Security Version |
|----------|------|---------|------------------|
| **HTTP** | 80 | Web traffic | HTTPS (443) |
| **FTP** | 21 | File transfer | SFTP (22) |
| **Telnet** | 23 | Remote access | SSH (22) |
| **SMTP** | 25 | Email sending | SMTPS (465/587) |

## 🌐 Network Services

### Domain Name System (DNS)
| Record Type | Purpose | Example | TTL |
|-------------|---------|---------|-----|
| **A** | IPv4 address | example.com → 192.168.1.1 | 3600 |
| **AAAA** | IPv6 address | example.com → 2001:db8::1 | 3600 |
| **CNAME** | Alias | www → example.com | 300 |
| **MX** | Mail server | mail.example.com | 3600 |
| **TXT** | Text records | SPF, DKIM | 300 |

### Dynamic Host Configuration Protocol (DHCP)
| Component | Function | Configuration |
|-----------|----------|---------------|
| **Scope** | IP range | 192.168.1.100-200 |
| **Lease Time** | IP duration | 24 hours |
| **Options** | Additional config | DNS, gateway |
| **Reservations** | Static assignments | MAC → IP mapping |

### Network Time Protocol (NTP)
| Stratum | Source | Accuracy | Examples |
|---------|--------|----------|----------|
| **0** | Reference clock | Microseconds | GPS, atomic clock |
| **1** | Primary servers | Milliseconds | pool.ntp.org |
| **2** | Secondary servers | Milliseconds | ISP NTP servers |
| **3+** | Client systems | Variable | Local systems |

## 🔒 Network Security

### Access Control Lists (ACLs)
| Type | Placement | Granularity | Use Cases |
|------|-----------|-------------|-----------|
| **Standard** | Close to destination | Source IP only | Basic filtering |
| **Extended** | Close to source | Source, dest, port, protocol | Detailed control |
| **Named** | Flexible | Descriptive names | Complex policies |
| **Time-based** | Scheduled | Time restrictions | Business hours |

### Virtual Private Networks (VPNs)
| Type | Protocol | Security | Use Cases |
|------|----------|---------|-----------|
| **Site-to-Site** | IPSec | High | Office connectivity |
| **Remote Access** | SSL/TLS, IPSec | Medium-High | Remote workers |
| **MPLS VPN** | BGP/MPLS | High | Enterprise WAN |
| **SD-WAN** | Various | Medium-High | Cloud connectivity |

### Network Segmentation
| Method | Implementation | Security Level | Complexity |
|--------|----------------|----------------|------------|
| **VLANs** | Switch configuration | Medium | Low |
| **Subnets** | Router/firewall | Medium | Medium |
| **Microsegmentation** | Software-defined | High | High |
| **Zero Trust** | Identity-based | Very High | Very High |

## 📶 Wireless Networking

### Wi-Fi Standards
| Standard | Speed | Frequency | Range | Year |
|----------|-------|-----------|-------|------|
| **802.11n** | 600 Mbps | 2.4/5 GHz | Good | 2009 |
| **802.11ac** | 6.93 Gbps | 5 GHz | Good | 2013 |
| **802.11ax (Wi-Fi 6)** | 9.6 Gbps | 2.4/5 GHz | Better | 2019 |
| **802.11ax (Wi-Fi 6E)** | 9.6 Gbps | 2.4/5/6 GHz | Better | 2020 |
| **802.11be (Wi-Fi 7)** | 46 Gbps | 2.4/5/6 GHz | Best | 2024 |

### Wireless Security
| Protocol | Security Level | Encryption | Vulnerabilities |
|----------|----------------|------------|-----------------|
| **WEP** | Very Low | RC4 | Easily cracked |
| **WPA** | Low | TKIP | Dictionary attacks |
| **WPA2** | Medium | AES | KRACK attack |
| **WPA3** | High | AES + SAE | Current standard |

### Enterprise Wireless
| Feature | Purpose | Implementation |
|---------|---------|----------------|
| **802.1X** | Authentication | RADIUS server |
| **RADIUS** | Centralized auth | FreeRADIUS, Microsoft NPS |
| **Captive Portal** | Guest access | Web-based login |
| **Band Steering** | Load balancing | 5GHz preference |

## 📊 Network Monitoring

### Monitoring Protocols
| Protocol | Purpose | Information | Tools |
|----------|---------|-------------|-------|
| **SNMP** | Device monitoring | Performance metrics | Nagios, PRTG |
| **NetFlow** | Traffic analysis | Flow information | SolarWinds, Plixer |
| **sFlow** | Packet sampling | Network visibility | InMon, Ntopng |
| **IPFIX** | Flow export | Standardized flows | Various vendors |

### Network Monitoring Tools
| Tool | Type | Features | Cost |
|------|------|----------|------|
| **Nagios** | Open source | Alerting, plugins | Free |
| **PRTG** | Commercial | Easy setup, sensors | Paid |
| **SolarWinds** | Enterprise | Comprehensive suite | Expensive |
| **Zabbix** | Open source | Scalable monitoring | Free |
| **LibreNMS** | Open source | Auto-discovery | Free |

### Performance Metrics
| Metric | Description | Normal Range | Tools |
|--------|-------------|--------------|-------|
| **Bandwidth Utilization** | Link usage percentage | <80% | MRTG, Cacti |
| **Latency** | Round-trip time | <100ms LAN | Ping, traceroute |
| **Packet Loss** | Dropped packets | <1% | Ping, iperf |
| **Jitter** | Latency variation | <30ms | VoIP tools |

## 🔄 Software-Defined Networking

### SDN Architecture
| Layer | Components | Function | Examples |
|-------|------------|----------|----------|
| **Application** | Network apps | Business logic | Load balancers |
| **Control** | SDN controller | Network intelligence | OpenDaylight |
| **Infrastructure** | Network devices | Packet forwarding | OpenFlow switches |

### SDN Controllers
| Controller | Language | Features | Use Cases |
|------------|----------|----------|-----------|
| **OpenDaylight** | Java | Modular, extensible | Enterprise SDN |
| **ONOS** | Java | Carrier-grade | Service providers |
| **Floodlight** | Java | Simple, lightweight | Research, education |
| **Ryu** | Python | Component-based | Development |

### Network Function Virtualization (NFV)
| Function | Traditional | Virtualized | Benefits |
|----------|-------------|-------------|---------|
| **Firewall** | Hardware appliance | VM/container | Flexibility, cost |
| **Load Balancer** | Dedicated device | Software | Scalability |
| **Router** | Physical router | Virtual router | Agility |
| **WAN Optimizer** | Appliance | VNF | Deployment speed |

## 🤖 Network Automation

### Automation Tools
| Tool | Language | Approach | Use Cases |
|------|----------|----------|-----------|
| **Ansible** | YAML | Agentless | Configuration management |
| **Puppet** | Ruby DSL | Agent-based | Infrastructure automation |
| **Chef** | Ruby | Agent-based | Configuration management |
| **SaltStack** | Python | Agent/agentless | Event-driven automation |

### Network APIs
| Type | Protocol | Authentication | Examples |
|------|----------|----------------|----------|
| **REST** | HTTP/HTTPS | Token, OAuth | Cisco DNA Center |
| **NETCONF** | SSH/TLS | Username/password | Juniper devices |
| **RESTCONF** | HTTP/HTTPS | Basic, token | Modern network devices |
| **gRPC** | HTTP/2 | TLS certificates | Google network APIs |

### Infrastructure as Code
| Tool | Language | Focus | Cloud Support |
|------|----------|-------|---------------|
| **Terraform** | HCL | Multi-cloud | All major clouds |
| **CloudFormation** | JSON/YAML | AWS native | AWS only |
| **Pulumi** | Multiple languages | Developer-friendly | Multi-cloud |
| **ARM Templates** | JSON | Azure native | Azure only |

## 🏢 Enterprise Networking

### Campus Network Design
| Layer | Function | Devices | Redundancy |
|-------|----------|---------|------------|
| **Core** | High-speed backbone | Core switches | Full redundancy |
| **Distribution** | Policy enforcement | Layer 3 switches | Dual-homed |
| **Access** | End-device connectivity | Access switches | Uplink redundancy |

### WAN Technologies
| Technology | Speed | Distance | Cost | Use Cases |
|------------|-------|---------|------|-----------|
| **MPLS** | Variable | Global | High | Enterprise WAN |
| **SD-WAN** | Variable | Global | Medium | Cloud connectivity |
| **Ethernet** | 1G-100G | Metro | Medium | High bandwidth |
| **Internet VPN** | Variable | Global | Low | Small sites |

### Data Center Networking
| Architecture | Characteristics | Benefits | Challenges |
|--------------|----------------|----------|------------|
| **Three-Tier** | Core/Aggregation/Access | Familiar design | Oversubscription |
| **Spine-Leaf** | Full mesh | Predictable latency | Complexity |
| **Hyper-converged** | Integrated compute/storage | Simplicity | Vendor lock-in |

## 📱 Modern Networking Trends

### Intent-Based Networking (IBN)
- **Definition**: Network that captures business intent
- **Components**: Translation, activation, assurance
- **Benefits**: Automation, consistency, agility
- **Examples**: Cisco DNA, Juniper Contrail

### Network as a Service (NaaS)
- **Model**: Consumption-based networking
- **Benefits**: OpEx vs CapEx, scalability
- **Providers**: Cisco, HPE, cloud providers
- **Use Cases**: Branch networking, data center

### 5G and Edge Computing
- **Ultra-low latency**: <1ms applications
- **Edge data centers**: Distributed computing
- **Network slicing**: Dedicated virtual networks
- **Use cases**: IoT, autonomous vehicles, AR/VR

## 🎯 Network Career Paths

### Entry Level
| Role | Responsibilities | Skills | Certifications |
|------|-----------------|--------|----------------|
| **Network Technician** | Cable installation, basic troubleshooting | Hardware, cabling | Network+ |
| **Help Desk** | User support, basic networking | Customer service, basics | A+ |
| **Junior Admin** | Device configuration, monitoring | CLI, protocols | CCNA |

### Mid Level
| Role | Responsibilities | Skills | Certifications |
|------|-----------------|--------|----------------|
| **Network Engineer** | Design, implementation | Routing, switching | CCNP, JNCIA |
| **Security Engineer** | Firewall, VPN management | Security protocols | CCNA Security |
| **Wireless Engineer** | Wi-Fi design, troubleshooting | RF, wireless protocols | CWNA |

### Senior Level
| Role | Responsibilities | Skills | Experience |
|------|-----------------|--------|-----------|
| **Network Architect** | Network design, strategy | Architecture, business | 7+ years |
| **Principal Engineer** | Technical leadership | Deep expertise | 10+ years |
| **Network Manager** | Team leadership, budgets | Management, technical | 5+ years |

## 📚 Learning Resources

### Certifications
| Vendor | Entry | Professional | Expert |
|--------|-------|--------------|--------|
| **Cisco** | CCNA | CCNP | CCIE |
| **Juniper** | JNCIA | JNCIP | JNCIE |
| **CompTIA** | Network+ | Security+ | Advanced Security |
| **Vendor Neutral** | Network+ | CISSP | CCIE/JNCIE |

### Training Platforms
- **Cisco Networking Academy** - Comprehensive networking courses
- **Juniper Learning Portal** - Juniper-specific training
- **CBT Nuggets** - Video-based IT training
- **INE** - Expert-level networking training
- **Pluralsight** - Technology skills platform

### Hands-On Labs
- **GNS3** - Network simulation software
- **EVE-NG** - Emulated virtual environment
- **Packet Tracer** - Cisco network simulator
- **VIRL** - Cisco virtual internet routing lab
- **Containerlab** - Container-based network labs

### Books & Resources
- **Network Warrior** - Gary Donahue
- **TCP/IP Illustrated** - W. Richard Stevens
- **Computer Networks** - Andrew Tanenbaum
- **Routing TCP/IP** - Jeff Doyle
- **Network Security Essentials** - William Stallings

---

*Cập nhật lần cuối: December 2024*