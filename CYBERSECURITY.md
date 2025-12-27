# Tổng Hợp Cybersecurity & Information Security

## 📋 Mục Lục
- [Security Frameworks & Standards](#security-frameworks--standards)
- [Network Security](#network-security)
- [Application Security](#application-security)
- [Identity & Access Management](#identity--access-management)
- [Endpoint Security](#endpoint-security)
- [Cloud Security](#cloud-security)
- [Security Testing Tools](#security-testing-tools)
- [Incident Response & Forensics](#incident-response--forensics)
- [Compliance & Governance](#compliance--governance)

## 🛡️ Security Frameworks & Standards

### International Standards
| Framework | Organization | Focus | Use Cases |
|-----------|--------------|-------|-----------|
| **ISO 27001** | ISO | Information Security Management | Enterprise security management |
| **NIST Cybersecurity Framework** | NIST | Risk management | US government, enterprises |
| **CIS Controls** | Center for Internet Security | Security controls | Practical security implementation |
| **COBIT** | ISACA | IT governance | IT governance and management |
| **ITIL** | Axelos | IT service management | Service delivery |

### Industry-Specific Frameworks
| Framework | Industry | Requirements | Compliance |
|-----------|----------|--------------|------------|
| **PCI DSS** | Payment cards | Card data protection | Mandatory for card processors |
| **HIPAA** | Healthcare | Health data protection | US healthcare |
| **SOX** | Finance | Financial reporting | Public companies |
| **GDPR** | General | Data privacy | EU data processing |
| **FISMA** | Government | Federal systems | US federal agencies |

### Security Maturity Models
| Model | Purpose | Levels | Use Cases |
|-------|---------|--------|-----------|
| **CMMI** | Process improvement | 5 levels | Software development |
| **BSIMM** | Security maturity | Descriptive model | Security program assessment |
| **SAMM** | Software security | 4 business functions | Secure development |

## 🌐 Network Security

### Firewalls & Network Protection
| Type | Examples | Ưu điểm | Nhược điểm | Use Cases |
|------|----------|---------|------------|-----------|
| **Next-Gen Firewalls** | Palo Alto, Fortinet, Check Point | Deep packet inspection, app awareness | Cost, complexity | Enterprise perimeter |
| **Web Application Firewalls** | Cloudflare, AWS WAF, F5 | HTTP/HTTPS protection | Application-specific | Web application protection |
| **Network Firewalls** | pfSense, OPNsense, iptables | Cost-effective, customizable | Limited features | SMB, home networks |
| **Cloud Firewalls** | AWS Security Groups, Azure NSG | Cloud-native, scalable | Cloud-specific | Cloud workloads |

### Network Monitoring & Detection
| Tool | Type | Features | Use Cases |
|------|------|----------|-----------|
| **Wireshark** | Packet analyzer | Deep packet inspection | Network troubleshooting |
| **Nmap** | Network scanner | Port scanning, OS detection | Network discovery |
| **Snort** | IDS/IPS | Signature-based detection | Intrusion detection |
| **Suricata** | IDS/IPS | Multi-threaded, Lua scripting | High-performance detection |
| **Zeek (Bro)** | Network monitor | Protocol analysis | Network security monitoring |

### VPN & Remote Access
| Type | Solutions | Security Level | Use Cases |
|------|-----------|----------------|-----------|
| **Site-to-Site VPN** | IPSec, WireGuard | High | Office connectivity |
| **Remote Access VPN** | OpenVPN, Cisco AnyConnect | Medium-High | Remote workers |
| **Zero Trust Network Access** | Zscaler, Cloudflare Access | Very High | Modern remote access |
| **Software-Defined Perimeter** | Perimeter 81, Cato Networks | High | Cloud-first organizations |

## 🔐 Application Security

### Static Application Security Testing (SAST)
| Tool | Languages | Features | Deployment |
|------|-----------|----------|------------|
| **SonarQube** | 25+ languages | Code quality + security | Self-hosted/Cloud |
| **Checkmarx** | 22+ languages | Enterprise features | Enterprise |
| **Veracode** | Multiple | Cloud-based scanning | SaaS |
| **Semgrep** | 17+ languages | Fast, customizable rules | Open source/Commercial |

### Dynamic Application Security Testing (DAST)
| Tool | Type | Features | Use Cases |
|------|------|----------|-----------|
| **OWASP ZAP** | Open source | Automated + manual testing | Web application testing |
| **Burp Suite** | Commercial | Professional web testing | Penetration testing |
| **Nessus** | Vulnerability scanner | Network + web scanning | Comprehensive scanning |
| **Acunetix** | Web scanner | Automated web scanning | Web application security |

### Interactive Application Security Testing (IAST)
| Tool | Approach | Benefits | Limitations |
|------|---------|----------|-------------|
| **Contrast Security** | Runtime analysis | Real-time detection | Performance impact |
| **Seeker** | Interactive testing | Accurate results | Complex setup |
| **Checkmarx IAST** | Hybrid approach | Comprehensive coverage | Cost |

### Software Composition Analysis (SCA)
| Tool | Focus | Features | Integration |
|------|-------|----------|-------------|
| **Snyk** | Open source vulnerabilities | Developer-friendly | CI/CD integration |
| **WhiteSource** | License + security | Policy enforcement | Enterprise integration |
| **Black Duck** | Open source management | Comprehensive scanning | Enterprise focus |
| **FOSSA** | License compliance | Legal risk management | Developer tools |

## 👤 Identity & Access Management

### Identity Providers
| Provider | Type | Features | Use Cases |
|----------|------|----------|-----------|
| **Active Directory** | On-premises | Windows integration | Enterprise Windows |
| **Azure AD** | Cloud | Microsoft ecosystem | Office 365, Azure |
| **Okta** | Cloud | Universal directory | Multi-cloud identity |
| **Auth0** | Developer-focused | Easy integration | Applications |
| **AWS Cognito** | Cloud | AWS integration | AWS applications |

### Multi-Factor Authentication
| Solution | Methods | Integration | Use Cases |
|----------|---------|-------------|-----------|
| **Microsoft Authenticator** | Push, TOTP, SMS | Microsoft ecosystem | Office 365 users |
| **Google Authenticator** | TOTP | Wide compatibility | General use |
| **Authy** | TOTP, push | Multi-device sync | Personal/business |
| **YubiKey** | Hardware token | High security | High-security environments |
| **RSA SecurID** | Hardware/software token | Enterprise features | Enterprise |

### Privileged Access Management
| Solution | Features | Use Cases |
|----------|----------|-----------|
| **CyberArk** | Enterprise PAM | Large enterprises |
| **BeyondTrust** | Privileged remote access | IT administration |
| **Thycotic** | Secret management | Password management |
| **HashiCorp Vault** | Secrets management | DevOps, cloud-native |

## 💻 Endpoint Security

### Antivirus & Anti-Malware
| Solution | Type | Features | Target Market |
|----------|------|----------|---------------|
| **Windows Defender** | Built-in | Free, integrated | Windows users |
| **Bitdefender** | Commercial | High detection rates | Consumer/business |
| **Kaspersky** | Commercial | Advanced threat protection | Global market |
| **CrowdStrike Falcon** | Cloud-native EDR | AI-powered detection | Enterprise |
| **SentinelOne** | Next-gen endpoint | Autonomous response | Enterprise |

### Endpoint Detection & Response (EDR)
| Solution | Approach | Strengths | Use Cases |
|----------|----------|-----------|-----------|
| **CrowdStrike** | Cloud-native | Threat hunting, AI | Enterprise security |
| **Carbon Black** | Behavioral analysis | Incident response | Security teams |
| **Microsoft Defender ATP** | Integrated | Windows integration | Microsoft environments |
| **Cylance** | AI-based | Predictive prevention | Proactive security |

### Mobile Device Management
| Solution | Platform | Features | Use Cases |
|----------|----------|----------|-----------|
| **Microsoft Intune** | Cross-platform | Office 365 integration | Enterprise mobility |
| **VMware Workspace ONE** | Multi-platform | Unified endpoint management | Large enterprises |
| **Jamf** | Apple-focused | Mac/iOS management | Apple environments |
| **MobileIron** | Enterprise | Security-focused | BYOD policies |

## ☁️ Cloud Security

### Cloud Security Posture Management
| Tool | Cloud Support | Features | Use Cases |
|------|---------------|----------|-----------|
| **Prisma Cloud** | Multi-cloud | Compliance, vulnerability management | Enterprise cloud security |
| **CloudGuard** | Multi-cloud | Threat prevention | Check Point customers |
| **Dome9** | Multi-cloud | Continuous compliance | Cloud compliance |
| **AWS Security Hub** | AWS | Centralized security findings | AWS environments |

### Cloud Access Security Brokers (CASB)
| Solution | Deployment | Features | Use Cases |
|----------|------------|----------|-----------|
| **Microsoft Cloud App Security** | Cloud | Office 365 integration | Microsoft environments |
| **Netskope** | Cloud/On-premises | DLP, threat protection | Enterprise cloud usage |
| **Forcepoint CASB** | Hybrid | Data protection | Data-sensitive organizations |
| **Symantec CloudSOC** | Cloud | Cloud app visibility | Cloud governance |

### Container Security
| Tool | Focus | Features | Integration |
|------|-------|----------|-------------|
| **Twistlock/Prisma Cloud** | Full lifecycle | Vulnerability management | CI/CD integration |
| **Aqua Security** | Runtime protection | Behavioral monitoring | Kubernetes |
| **Sysdig Secure** | Runtime security | Compliance, forensics | Cloud-native |
| **Anchore** | Image scanning | Policy-based scanning | DevOps pipelines |

## 🔍 Security Testing Tools

### Vulnerability Scanners
| Tool | Type | Strengths | Use Cases |
|------|------|-----------|-----------|
| **Nessus** | Network scanner | Comprehensive coverage | Infrastructure scanning |
| **OpenVAS** | Open source | Free, extensible | Budget-conscious organizations |
| **Qualys VMDR** | Cloud-based | Continuous monitoring | Enterprise vulnerability management |
| **Rapid7 Nexpose** | Enterprise | Integration capabilities | Large-scale scanning |

### Penetration Testing Tools
| Tool | Category | Features | Skill Level |
|------|----------|----------|-------------|
| **Metasploit** | Exploitation framework | Extensive exploit database | Intermediate-Advanced |
| **Kali Linux** | Penetration testing OS | 600+ security tools | Beginner-Advanced |
| **Cobalt Strike** | Red team platform | Advanced persistent threats | Advanced |
| **Empire** | Post-exploitation | PowerShell agents | Intermediate |

### Web Application Testing
| Tool | Type | Strengths | Target Users |
|------|------|-----------|-------------|
| **Burp Suite** | Web proxy | Manual testing capabilities | Security professionals |
| **OWASP ZAP** | Open source | Free, community-driven | Everyone |
| **Nikto** | Web scanner | Quick vulnerability detection | System administrators |
| **SQLmap** | SQL injection | Automated SQL injection testing | Penetration testers |

## 🚨 Incident Response & Forensics

### Security Information & Event Management (SIEM)
| Solution | Deployment | Strengths | Use Cases |
|----------|------------|-----------|-----------|
| **Splunk** | On-premises/Cloud | Powerful search, analytics | Large enterprises |
| **IBM QRadar** | On-premises/Cloud | AI-powered analysis | Enterprise security |
| **ArcSight** | On-premises | Correlation rules | Large-scale monitoring |
| **Elastic Security** | Open source/Commercial | Open source flexibility | Cost-conscious organizations |

### Security Orchestration (SOAR)
| Platform | Integration | Automation | Use Cases |
|----------|-------------|------------|-----------|
| **Phantom (Splunk)** | 300+ integrations | Playbook automation | Splunk environments |
| **Demisto (Palo Alto)** | Extensive integrations | Machine learning | Enterprise security |
| **IBM Resilient** | IBM ecosystem | Case management | IBM customers |
| **Swimlane** | API-first | Visual playbooks | Mid-market |

### Digital Forensics
| Tool | Type | Capabilities | Use Cases |
|------|------|-------------|-----------|
| **EnCase** | Commercial | Comprehensive forensics | Law enforcement |
| **FTK (Forensic Toolkit)** | Commercial | Fast processing | Corporate investigations |
| **Autopsy** | Open source | Timeline analysis | Budget forensics |
| **Volatility** | Memory analysis | RAM forensics | Malware analysis |

### Threat Intelligence
| Platform | Focus | Data Sources | Use Cases |
|----------|-------|--------------|-----------|
| **ThreatConnect** | Threat intelligence | Multiple feeds | Threat hunting |
| **Recorded Future** | Predictive intelligence | Web intelligence | Proactive security |
| **Anomali** | Threat intelligence | Community sharing | Collaborative defense |
| **MISP** | Open source | Information sharing | Community-driven |

## 📋 Compliance & Governance

### Governance, Risk & Compliance (GRC)
| Solution | Focus | Features | Target Market |
|----------|-------|----------|---------------|
| **ServiceNow GRC** | Enterprise GRC | Integrated platform | Large enterprises |
| **RSA Archer** | Risk management | Customizable workflows | Enterprise risk |
| **MetricStream** | Compliance management | Regulatory compliance | Regulated industries |
| **LogicGate** | Risk management | Modern interface | Mid-market |

### Data Loss Prevention (DLP)
| Solution | Deployment | Strengths | Use Cases |
|----------|------------|-----------|-----------|
| **Symantec DLP** | Hybrid | Comprehensive coverage | Enterprise data protection |
| **Forcepoint DLP** | Cloud/On-premises | Behavioral analysis | Human-centric security |
| **Microsoft Purview** | Cloud | Office 365 integration | Microsoft environments |
| **Digital Guardian** | Endpoint-focused | Data visibility | Insider threat protection |

### Privacy Management
| Tool | Focus | Capabilities | Compliance |
|------|-------|-------------|------------|
| **OneTrust** | Privacy management | GDPR, CCPA compliance | Global privacy |
| **TrustArc** | Privacy platform | Risk assessment | Privacy compliance |
| **Nymity** | Privacy program management | Privacy impact assessments | Enterprise privacy |

## 🎯 Security Career Paths

### Entry Level Roles
| Role | Responsibilities | Skills Needed | Certifications |
|------|-----------------|---------------|----------------|
| **Security Analyst** | Monitor, investigate incidents | SIEM, networking | Security+, CySA+ |
| **Junior Penetration Tester** | Basic vulnerability testing | Scripting, tools | CEH, OSCP |
| **Compliance Analyst** | Audit, documentation | Frameworks, documentation | CISA, CISM |

### Mid-Level Roles
| Role | Responsibilities | Skills Needed | Certifications |
|------|-----------------|---------------|----------------|
| **Security Engineer** | Design, implement security | Architecture, automation | CISSP, CCSP |
| **Incident Response Specialist** | Handle security incidents | Forensics, malware analysis | GCIH, GCFA |
| **Security Architect** | Design security solutions | Enterprise architecture | SABSA, TOGAF |

### Senior Level Roles
| Role | Responsibilities | Skills Needed | Experience |
|------|-----------------|---------------|------------|
| **CISO** | Security strategy, leadership | Business, leadership | 10+ years |
| **Security Consultant** | Advisory, implementation | Broad expertise | 7+ years |
| **Red Team Lead** | Advanced testing, research | Advanced techniques | 5+ years |

## 📊 Security Metrics & KPIs

### Technical Metrics
| Metric | Purpose | Measurement |
|--------|---------|-------------|
| **Mean Time to Detection (MTTD)** | Incident response efficiency | Hours/days |
| **Mean Time to Response (MTTR)** | Response effectiveness | Hours/days |
| **Vulnerability Remediation Time** | Patch management | Days/weeks |
| **Security Training Completion** | Awareness program | Percentage |

### Business Metrics
| Metric | Business Value | Reporting |
|--------|---------------|----------|
| **Security ROI** | Investment justification | Financial impact |
| **Compliance Score** | Regulatory adherence | Percentage |
| **Risk Reduction** | Risk management | Risk score |
| **Security Incidents** | Program effectiveness | Count/trend |

## 🔮 Emerging Security Trends

### Zero Trust Architecture
- **Principles**: Never trust, always verify
- **Components**: Identity, device, network, application
- **Implementation**: Gradual migration approach
- **Benefits**: Reduced attack surface, better visibility

### AI/ML in Security
- **Threat Detection**: Behavioral analysis, anomaly detection
- **Automation**: Response orchestration, threat hunting
- **Challenges**: False positives, adversarial AI
- **Future**: Autonomous security operations

### Cloud-Native Security
- **DevSecOps**: Security in CI/CD pipelines
- **Container Security**: Runtime protection, image scanning
- **Serverless Security**: Function-level security
- **Infrastructure as Code**: Security policy as code

## 📚 Learning Resources

### Certifications
| Level | Certifications | Focus |
|-------|----------------|-------|
| **Entry** | Security+, Network+, CySA+ | Fundamentals |
| **Intermediate** | CEH, GCIH, CISSP | Specialized skills |
| **Advanced** | OSCP, CISSP, CISM | Expert level |
| **Management** | CISA, CISM, CISSP | Leadership |

### Training Platforms
- **Cybrary** - Free cybersecurity training
- **SANS** - Premium security training
- **Coursera** - University cybersecurity courses
- **Udemy** - Affordable security courses
- **Pluralsight** - Technology skills platform

### Hands-On Practice
- **TryHackMe** - Beginner-friendly challenges
- **Hack The Box** - Advanced penetration testing
- **VulnHub** - Vulnerable VMs for practice
- **OverTheWire** - Wargames and challenges
- **PentesterLab** - Web application security

---

*Cập nhật lần cuối: December 2024*