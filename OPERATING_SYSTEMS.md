# Tổng Hợp Hệ Điều Hành & System Administration

## 📋 Mục Lục
- [Desktop Operating Systems](#desktop-operating-systems)
- [Server Operating Systems](#server-operating-systems)
- [Mobile Operating Systems](#mobile-operating-systems)
- [Embedded & Real-Time Systems](#embedded--real-time-systems)
- [Virtualization & Containers](#virtualization--containers)
- [System Administration](#system-administration)
- [Performance & Monitoring](#performance--monitoring)
- [Security & Hardening](#security--hardening)
- [Automation & Scripting](#automation--scripting)

## 🖥️ Desktop Operating Systems

### Windows Family
| Version | Release Year | Support Status | Target Users | Key Features |
|---------|--------------|----------------|--------------|--------------|
| **Windows 11** | 2021 | Current | Consumer/Enterprise | Modern UI, Teams integration, enhanced security |
| **Windows 10** | 2015 | Extended support until 2025 | Consumer/Enterprise | Universal apps, Cortana, Windows Hello |
| **Windows Server 2022** | 2021 | Current | Enterprise | Hybrid cloud, containers, security |
| **Windows Server 2019** | 2018 | Mainstream support | Enterprise | Kubernetes, Linux containers |

### macOS Versions
| Version | Codename | Release Year | Hardware Support | Notable Features |
|---------|----------|--------------|------------------|------------------|
| **macOS Sonoma** | 14.x | 2023 | Apple Silicon/Intel | Interactive widgets, Game Mode |
| **macOS Ventura** | 13.x | 2022 | Apple Silicon/Intel | Stage Manager, Continuity Camera |
| **macOS Monterey** | 12.x | 2021 | Apple Silicon/Intel | Universal Control, AirPlay to Mac |
| **macOS Big Sur** | 11.x | 2020 | Apple Silicon/Intel | iOS app support, redesigned UI |

### Linux Desktop Distributions
| Distribution | Base | Desktop Environment | Target Users | Package Manager |
|--------------|------|-------------------|--------------|-----------------|
| **Ubuntu** | Debian | GNOME | Beginners | APT |
| **Linux Mint** | Ubuntu | Cinnamon/MATE | Windows migrants | APT |
| **Fedora** | Red Hat | GNOME | Developers | DNF |
| **openSUSE** | Independent | KDE/GNOME | Enterprise users | Zypper |
| **Arch Linux** | Independent | Various | Advanced users | Pacman |
| **Elementary OS** | Ubuntu | Pantheon | macOS-like experience | APT |

## 🖧 Server Operating Systems

### Linux Server Distributions
| Distribution | Base | Release Cycle | Support | Use Cases |
|--------------|------|---------------|---------|-----------|
| **Ubuntu Server** | Debian | 6 months (LTS: 2 years) | 5-10 years | Cloud, containers, general purpose |
| **Red Hat Enterprise Linux** | Fedora | ~3 years | 10 years | Enterprise, mission-critical |
| **CentOS Stream** | RHEL upstream | Rolling | Community | Development, testing |
| **SUSE Linux Enterprise** | openSUSE | ~4 years | 13 years | Enterprise, SAP workloads |
| **Debian** | Independent | ~2 years | 3-5 years | Stability, servers |
| **Amazon Linux** | RHEL-based | Rolling | AWS support | AWS workloads |

### Windows Server Editions
| Edition | Target | Features | Licensing |
|---------|--------|----------|-----------|
| **Standard** | Small-medium business | 2 VMs, basic features | Per core |
| **Datacenter** | Large enterprise | Unlimited VMs, advanced features | Per core |
| **Essentials** | Small business | 25 users, basic features | Per server |
| **Core** | Minimal installation | Command line only | Same as full |

### Unix-like Systems
| System | Vendor | Architecture | Use Cases |
|--------|--------|--------------|-----------|
| **AIX** | IBM | POWER | Enterprise, mainframes |
| **Solaris** | Oracle | SPARC/x86 | Enterprise, databases |
| **FreeBSD** | Community | x86/ARM | Servers, networking |
| **OpenBSD** | Community | Multiple | Security-focused |
| **NetBSD** | Community | Multiple | Portability |

## 📱 Mobile Operating Systems

### Smartphone Operating Systems
| OS | Developer | Market Share | Programming Languages | App Store |
|----|-----------|--------------|----------------------|-----------|
| **Android** | Google | ~71% | Java, Kotlin, C++ | Google Play Store |
| **iOS** | Apple | ~28% | Swift, Objective-C | App Store |
| **HarmonyOS** | Huawei | ~2% | JavaScript, Java | AppGallery |
| **KaiOS** | KaiOS Technologies | <1% | HTML5, JavaScript | KaiStore |

### Tablet Operating Systems
| OS | Base | Devices | Features |
|----|------|---------|----------|
| **iPadOS** | iOS | iPad | Desktop-class apps, multitasking |
| **Android** | Linux | Various tablets | Flexible UI, Google services |
| **Windows 11** | NT kernel | Surface, 2-in-1s | Full desktop compatibility |
| **ChromeOS** | Linux | Chromebooks | Web-based, Android app support |

### Wearable Operating Systems
| OS | Developer | Devices | Capabilities |
|----|-----------|---------|--------------|
| **watchOS** | Apple | Apple Watch | Health, fitness, apps |
| **Wear OS** | Google | Various smartwatches | Google services, fitness |
| **Tizen** | Samsung | Galaxy Watch | Samsung ecosystem |
| **Fitbit OS** | Google | Fitbit devices | Fitness-focused |

## ⚡ Embedded & Real-Time Systems

### Real-Time Operating Systems (RTOS)
| RTOS | Developer | Architecture | Use Cases |
|------|-----------|--------------|-----------|
| **FreeRTOS** | Amazon | Microcontroller | IoT, embedded systems |
| **VxWorks** | Wind River | Multiple | Aerospace, automotive |
| **QNX** | BlackBerry | Microkernel | Automotive, medical |
| **ThreadX** | Microsoft | Microcontroller | IoT, industrial |
| **Zephyr** | Linux Foundation | Multiple | IoT, connected devices |

### Embedded Linux
| Distribution | Target | Features | Use Cases |
|--------------|--------|----------|-----------|
| **Yocto Project** | Custom builds | Build system | Industrial, automotive |
| **Buildroot** | Simple builds | Lightweight | Simple embedded systems |
| **OpenWrt** | Routers | Network focus | Home routers, networking |
| **Raspbian/Raspberry Pi OS** | Raspberry Pi | Educational | Learning, prototyping |

### IoT Operating Systems
| OS | Developer | Connectivity | Power Management |
|----|-----------|--------------|------------------|
| **Contiki** | Community | 6LoWPAN, CoAP | Ultra-low power |
| **RIOT** | Community | Multiple protocols | Energy efficient |
| **Mbed OS** | ARM | Cellular, Wi-Fi, LoRa | Power optimization |
| **Amazon FreeRTOS** | Amazon | AWS IoT integration | Cloud connectivity |

## 🔄 Virtualization & Containers

### Hypervisors
| Type | Product | Vendor | Architecture | Use Cases |
|------|---------|--------|--------------|-----------|
| **Type 1** | VMware vSphere | VMware | Bare metal | Enterprise virtualization |
| **Type 1** | Microsoft Hyper-V | Microsoft | Bare metal | Windows environments |
| **Type 1** | Citrix XenServer | Citrix | Bare metal | VDI, cloud |
| **Type 2** | VMware Workstation | VMware | Hosted | Development, testing |
| **Type 2** | VirtualBox | Oracle | Hosted | Personal use, testing |

### Container Platforms
| Platform | Developer | Container Runtime | Orchestration |
|----------|-----------|-------------------|---------------|
| **Docker** | Docker Inc. | containerd | Docker Swarm |
| **Podman** | Red Hat | CRI-O | Kubernetes |
| **LXC/LXD** | Canonical | LXC | Built-in |
| **rkt** | CoreOS (deprecated) | rkt | Kubernetes |

### Container Orchestration
| Platform | Developer | Architecture | Use Cases |
|----------|-----------|--------------|-----------|
| **Kubernetes** | CNCF | Master/worker nodes | Production container orchestration |
| **Docker Swarm** | Docker | Manager/worker nodes | Simple container orchestration |
| **Apache Mesos** | Apache | Master/agent | Large-scale resource management |
| **Nomad** | HashiCorp | Server/client | Multi-workload orchestration |

## ⚙️ System Administration

### Package Management
| OS Family | Package Manager | Package Format | Repository |
|-----------|-----------------|----------------|------------|
| **Debian/Ubuntu** | APT | .deb | apt repositories |
| **Red Hat/CentOS** | YUM/DNF | .rpm | yum repositories |
| **SUSE** | Zypper | .rpm | zypper repositories |
| **Arch** | Pacman | .pkg.tar.xz | pacman repositories |
| **macOS** | Homebrew | Formulae | Homebrew taps |
| **Windows** | Chocolatey/winget | .nupkg/.msix | Package repositories |

### Service Management
| OS | Service Manager | Configuration | Commands |
|----|-----------------|---------------|----------|
| **Modern Linux** | systemd | Unit files | systemctl |
| **Legacy Linux** | SysV Init | Init scripts | service |
| **macOS** | launchd | plist files | launchctl |
| **Windows** | Service Control Manager | Registry/Services.msc | sc, net |
| **FreeBSD** | rc | rc.conf | service |

### File Systems
| File System | OS Support | Features | Use Cases |
|-------------|------------|----------|-----------|
| **ext4** | Linux | Journaling, large files | Linux root filesystems |
| **XFS** | Linux, Unix | High performance, scalability | Large files, databases |
| **Btrfs** | Linux | Snapshots, compression | Modern Linux systems |
| **ZFS** | Solaris, FreeBSD, Linux | Snapshots, deduplication | Enterprise storage |
| **NTFS** | Windows | Permissions, compression | Windows systems |
| **APFS** | macOS, iOS | Encryption, snapshots | Apple devices |

### User & Permission Management
| OS | User Database | Permission Model | Tools |
|----|---------------|------------------|-------|
| **Linux/Unix** | /etc/passwd, LDAP | POSIX permissions, ACLs | useradd, chmod, setfacl |
| **Windows** | Active Directory, SAM | NTFS permissions, ACLs | User Manager, icacls |
| **macOS** | Directory Services | POSIX + ACLs | dscl, chmod |

## 📊 Performance & Monitoring

### System Monitoring Tools
| Tool | OS Support | Metrics | Interface |
|------|------------|---------|-----------|
| **htop** | Linux, macOS | CPU, memory, processes | Terminal |
| **Task Manager** | Windows | CPU, memory, disk, network | GUI |
| **Activity Monitor** | macOS | CPU, memory, energy | GUI |
| **iotop** | Linux | Disk I/O by process | Terminal |
| **nethogs** | Linux | Network usage by process | Terminal |

### Performance Analysis
| Category | Linux Tools | Windows Tools | Metrics |
|----------|-------------|---------------|---------|
| **CPU** | top, htop, sar | Task Manager, PerfMon | Usage, load average |
| **Memory** | free, vmstat | Task Manager, RAMMap | Usage, swap, cache |
| **Disk** | iostat, iotop | PerfMon, Resource Monitor | IOPS, throughput, latency |
| **Network** | ss, netstat, iftop | netstat, Resource Monitor | Connections, bandwidth |

### Log Management
| OS | Log Location | Log Format | Tools |
|----|--------------|------------|-------|
| **Linux** | /var/log | Text, syslog | journalctl, tail, grep |
| **Windows** | Event Viewer | Binary | Event Viewer, PowerShell |
| **macOS** | /var/log, Console | Text, binary | Console, log command |

### System Metrics
| Metric | Description | Normal Range | Monitoring |
|--------|-------------|--------------|------------|
| **CPU Usage** | Processor utilization | <80% sustained | Load average |
| **Memory Usage** | RAM utilization | <80% physical | Available memory |
| **Disk Usage** | Storage utilization | <90% capacity | Free space |
| **I/O Wait** | Disk bottleneck indicator | <20% | iostat |

## 🔒 Security & Hardening

### Access Control
| Method | Implementation | Granularity | Use Cases |
|--------|----------------|-------------|-----------|
| **Discretionary (DAC)** | File permissions | User/group/other | Standard Unix/Linux |
| **Mandatory (MAC)** | SELinux, AppArmor | System-wide policies | High-security environments |
| **Role-Based (RBAC)** | Windows, enterprise systems | Role assignments | Enterprise environments |
| **Attribute-Based (ABAC)** | Modern systems | Dynamic attributes | Complex authorization |

### Security Frameworks
| Framework | OS | Purpose | Implementation |
|-----------|----|---------|--------------| 
| **SELinux** | Linux | Mandatory access control | Red Hat, CentOS |
| **AppArmor** | Linux | Application confinement | Ubuntu, SUSE |
| **grsecurity** | Linux | Kernel hardening | Security-focused distributions |
| **Windows Defender** | Windows | Endpoint protection | Built-in Windows |

### Hardening Practices
| Area | Linux | Windows | Best Practices |
|------|-------|---------|----------------|
| **Updates** | apt update/upgrade | Windows Update | Regular patching |
| **Services** | Disable unnecessary | Services.msc | Minimal attack surface |
| **Firewall** | iptables, ufw | Windows Firewall | Default deny |
| **Accounts** | sudo, strong passwords | UAC, password policy | Principle of least privilege |

## 🤖 Automation & Scripting

### Shell Scripting
| Shell | OS | Strengths | Use Cases |
|-------|----|-----------| ---------|
| **Bash** | Linux, macOS | Powerful, ubiquitous | System administration |
| **PowerShell** | Windows, Linux, macOS | Object-oriented, .NET integration | Windows automation |
| **Zsh** | Linux, macOS | Advanced features, customizable | Interactive use |
| **Fish** | Linux, macOS | User-friendly, autocompletion | Interactive use |

### Configuration Management
| Tool | Approach | Language | Use Cases |
|------|----------|----------|-----------|
| **Ansible** | Agentless | YAML | Simple automation |
| **Puppet** | Agent-based | Ruby DSL | Enterprise configuration |
| **Chef** | Agent-based | Ruby | Infrastructure automation |
| **SaltStack** | Agent/agentless | Python/YAML | Event-driven automation |

### Infrastructure as Code
| Tool | Language | Cloud Support | Strengths |
|------|----------|---------------|-----------|
| **Terraform** | HCL | Multi-cloud | Declarative, state management |
| **CloudFormation** | JSON/YAML | AWS | AWS native |
| **Pulumi** | Multiple languages | Multi-cloud | Developer-friendly |
| **ARM Templates** | JSON | Azure | Azure native |

## 🎯 System Administration Career Path

### Entry Level Roles
| Role | Responsibilities | Skills Required | Certifications |
|------|-----------------|-----------------|----------------|
| **Help Desk Technician** | User support, basic troubleshooting | Customer service, basic IT | CompTIA A+ |
| **Junior System Administrator** | Basic server maintenance | OS basics, networking | Linux+, Server+ |
| **Desktop Support** | Workstation management | Hardware, OS installation | A+, Network+ |

### Mid-Level Roles
| Role | Responsibilities | Skills Required | Certifications |
|------|-----------------|-----------------|----------------|
| **System Administrator** | Server management, automation | Scripting, virtualization | RHCSA, MCSA |
| **Cloud Administrator** | Cloud infrastructure | Cloud platforms, automation | AWS SysOps, Azure Administrator |
| **DevOps Engineer** | CI/CD, infrastructure automation | Containers, orchestration | CKA, Docker Certified |

### Senior Level Roles
| Role | Responsibilities | Skills Required | Experience |
|------|-----------------|-----------------|-----------|
| **Senior System Architect** | Infrastructure design | Architecture, business alignment | 7+ years |
| **Site Reliability Engineer** | Production systems reliability | Programming, monitoring | 5+ years |
| **Infrastructure Manager** | Team leadership, strategy | Management, technical depth | 5+ years |

## 📈 Operating System Trends

### Current Trends
- **Containerization**: Docker, Kubernetes adoption
- **Cloud-Native**: Microservices, serverless
- **Edge Computing**: IoT, distributed systems
- **Security**: Zero-trust, immutable infrastructure
- **Automation**: Infrastructure as Code, GitOps

### Emerging Technologies
- **WebAssembly**: Cross-platform runtime
- **Unikernels**: Single-purpose OS images
- **Confidential Computing**: Hardware-based security
- **Quantum-Safe Cryptography**: Post-quantum security

### Future Outlook
- **AI Integration**: Intelligent system management
- **Sustainability**: Energy-efficient computing
- **Privacy**: Enhanced data protection
- **Interoperability**: Cross-platform compatibility

## 📚 Learning Resources

### Certifications
| Vendor | Entry Level | Professional | Expert |
|--------|-------------|--------------|--------|
| **CompTIA** | A+, Linux+ | Server+, Security+ | Advanced certifications |
| **Red Hat** | RHCSA | RHCE | RHCA |
| **Microsoft** | Azure Fundamentals | Azure Administrator | Azure Solutions Architect |
| **Linux Foundation** | LFCS | LFCE | CKA, CKS |

### Training Platforms
- **Linux Academy** - Linux and cloud training
- **Pluralsight** - Technology skills platform
- **CBT Nuggets** - IT training videos
- **Red Hat Training** - Official Red Hat courses
- **Microsoft Learn** - Free Microsoft training

### Hands-On Practice
- **VirtualBox/VMware** - Local virtualization
- **AWS Free Tier** - Cloud practice environment
- **DigitalOcean** - Affordable cloud VPS
- **Raspberry Pi** - Physical hardware learning
- **Docker** - Container technology practice

### Books & Documentation
- **UNIX and Linux System Administration Handbook** - Nemeth et al.
- **Windows Server Administration Fundamentals** - Microsoft
- **The Practice of System and Network Administration** - Limoncelli
- **Site Reliability Engineering** - Google
- **The Phoenix Project** - Gene Kim

---

*Cập nhật lần cuối: December 2024*