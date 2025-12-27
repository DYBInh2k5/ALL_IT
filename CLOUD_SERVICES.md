# Tổng Hợp Các Dịch Vụ Cloud Computing

## 📋 Mục Lục
- [Major Cloud Providers](#major-cloud-providers)
- [Compute Services](#compute-services)
- [Storage Services](#storage-services)
- [Database Services](#database-services)
- [Networking Services](#networking-services)
- [Serverless & Functions](#serverless--functions)
- [AI/ML Services](#aiml-services)
- [DevOps & Management](#devops--management)
- [Security Services](#security-services)

## 🏢 Major Cloud Providers

### Market Leaders
| Provider | Market Share | Strengths | Weaknesses | Best For |
|----------|--------------|-----------|------------|----------|
| **Amazon Web Services (AWS)** | ~32% | First mover, comprehensive services | Complex pricing, learning curve | Enterprise, startups, everything |
| **Microsoft Azure** | ~23% | Enterprise integration, hybrid cloud | Windows-centric perception | .NET apps, enterprises |
| **Google Cloud Platform** | ~10% | AI/ML, data analytics, Kubernetes | Smaller ecosystem | Data analytics, AI/ML |
| **Alibaba Cloud** | ~6% | Asia-Pacific dominance | Limited global presence | Asian markets |

### Regional & Specialized Providers
| Provider | Region/Specialty | Strengths | Use Cases |
|----------|------------------|-----------|-----------|
| **Oracle Cloud** | Enterprise databases | Database expertise | Oracle workloads |
| **IBM Cloud** | Enterprise, hybrid | Mainframe integration | Legacy modernization |
| **DigitalOcean** | Developers, SMBs | Simple, affordable | Small applications |
| **Linode** | Developers | Simple, good performance | Development, hosting |
| **Vultr** | Global infrastructure | Performance, pricing | Gaming, CDN |

## 💻 Compute Services

### Virtual Machines
| Provider | Service | Features | Use Cases |
|----------|---------|----------|-----------|
| **AWS** | EC2 | 400+ instance types, spot instances | General computing |
| **Azure** | Virtual Machines | Windows/Linux, hybrid benefits | Enterprise workloads |
| **GCP** | Compute Engine | Custom machine types, preemptible VMs | Flexible computing |
| **Alibaba** | ECS | Burstable instances, dedicated hosts | Asian workloads |

### Container Services
| Provider | Service | Type | Features |
|----------|---------|------|----------|
| **AWS** | ECS | Container orchestration | AWS-native, Fargate |
| **AWS** | EKS | Managed Kubernetes | Kubernetes-compatible |
| **Azure** | Container Instances | Serverless containers | Quick deployment |
| **Azure** | AKS | Managed Kubernetes | Azure integration |
| **GCP** | GKE | Managed Kubernetes | Autopilot mode |
| **GCP** | Cloud Run | Serverless containers | HTTP-triggered |

### Specialized Compute
| Service | Provider | Purpose | Use Cases |
|---------|----------|---------|-----------|
| **AWS Batch** | AWS | Batch processing | Scientific computing |
| **Azure Batch** | Azure | Parallel workloads | Rendering, simulation |
| **Google Cloud GPUs** | GCP | GPU computing | ML training, HPC |
| **AWS Graviton** | AWS | ARM-based processors | Cost optimization |

## 💾 Storage Services

### Object Storage
| Provider | Service | Features | Pricing Model |
|----------|---------|----------|---------------|
| **AWS** | S3 | Multiple storage classes, lifecycle | Pay per GB, requests |
| **Azure** | Blob Storage | Hot/cool/archive tiers | Tiered pricing |
| **GCP** | Cloud Storage | Multi-regional, nearline, coldline | Usage-based |
| **Alibaba** | Object Storage Service | Standard/IA/Archive | Tiered storage |

### Block Storage
| Provider | Service | Performance | Use Cases |
|----------|---------|-------------|-----------|
| **AWS** | EBS | Up to 64,000 IOPS | Database storage |
| **Azure** | Managed Disks | Premium SSD, Ultra SSD | High-performance apps |
| **GCP** | Persistent Disk | SSD, balanced, standard | VM storage |

### File Storage
| Provider | Service | Protocol | Use Cases |
|----------|---------|----------|-----------|
| **AWS** | EFS | NFS | Shared file systems |
| **Azure** | Files | SMB/NFS | Windows file shares |
| **GCP** | Filestore | NFS | High-performance file storage |

### Backup & Archive
| Service | Provider | Purpose | Retention |
|---------|----------|---------|-----------|
| **AWS Glacier** | AWS | Long-term archive | Years to decades |
| **Azure Archive** | Azure | Cold storage | Long-term backup |
| **Google Coldline** | GCP | Infrequent access | Quarterly access |

## 🗄️ Database Services

### Relational Databases
| Provider | Service | Engines | Features |
|----------|---------|---------|----------|
| **AWS** | RDS | MySQL, PostgreSQL, Oracle, SQL Server | Multi-AZ, read replicas |
| **AWS** | Aurora | MySQL, PostgreSQL compatible | Serverless, global |
| **Azure** | SQL Database | SQL Server | Elastic pools, hyperscale |
| **GCP** | Cloud SQL | MySQL, PostgreSQL, SQL Server | High availability |
| **GCP** | Spanner | Globally distributed SQL | ACID transactions |

### NoSQL Databases
| Provider | Service | Type | Use Cases |
|----------|---------|------|-----------|
| **AWS** | DynamoDB | Key-value/Document | Serverless applications |
| **Azure** | Cosmos DB | Multi-model | Global applications |
| **GCP** | Firestore | Document | Mobile/web apps |
| **GCP** | Bigtable | Wide-column | Analytics, IoT |

### Specialized Databases
| Service | Provider | Type | Use Cases |
|---------|----------|------|-----------|
| **Amazon Neptune** | AWS | Graph | Social networks |
| **Amazon Timestream** | AWS | Time-series | IoT monitoring |
| **Azure Database for PostgreSQL** | Azure | Managed PostgreSQL | Open source apps |
| **Google Cloud Memorystore** | GCP | In-memory | Caching, sessions |

## 🌐 Networking Services

### Content Delivery
| Provider | Service | Features | Global Presence |
|----------|---------|----------|-----------------|
| **AWS** | CloudFront | Edge locations, Lambda@Edge | 400+ locations |
| **Azure** | CDN | Microsoft/Verizon/Akamai | Global network |
| **GCP** | Cloud CDN | Google's global network | Google's edge |
| **Cloudflare** | CDN | Security, performance | 275+ cities |

### Load Balancing
| Provider | Service | Type | Features |
|----------|---------|------|----------|
| **AWS** | ALB/NLB | Application/Network | Auto scaling |
| **Azure** | Load Balancer | Layer 4/7 | Health probes |
| **GCP** | Cloud Load Balancing | Global/Regional | Anycast IPs |

### DNS & Domain
| Service | Provider | Features | Use Cases |
|---------|----------|----------|-----------|
| **Route 53** | AWS | Authoritative DNS, health checks | Domain management |
| **Azure DNS** | Azure | Anycast DNS | Azure integration |
| **Cloud DNS** | GCP | High performance | Google ecosystem |

### VPN & Connectivity
| Service | Provider | Type | Use Cases |
|---------|----------|------|-----------|
| **AWS VPN** | AWS | Site-to-site, client VPN | Hybrid connectivity |
| **Azure VPN Gateway** | Azure | Point-to-site, site-to-site | Hybrid cloud |
| **Cloud VPN** | GCP | IPsec VPN | Secure connections |
| **AWS Direct Connect** | AWS | Dedicated connection | High bandwidth |

## ⚡ Serverless & Functions

### Function as a Service (FaaS)
| Provider | Service | Runtime Support | Pricing Model |
|----------|---------|-----------------|---------------|
| **AWS** | Lambda | 15+ languages | Per request + duration |
| **Azure** | Functions | Multiple languages | Consumption/Premium |
| **GCP** | Cloud Functions | Node.js, Python, Go, Java | Per invocation |
| **Alibaba** | Function Compute | Multiple runtimes | Pay-per-use |

### Serverless Containers
| Service | Provider | Features | Use Cases |
|---------|----------|----------|-----------|
| **AWS Fargate** | AWS | Serverless containers | Microservices |
| **Azure Container Instances** | Azure | Quick container deployment | Batch jobs |
| **Google Cloud Run** | GCP | HTTP-triggered containers | Web services |

### Serverless Databases
| Service | Provider | Type | Scaling |
|---------|----------|------|---------|
| **Aurora Serverless** | AWS | Relational | Auto-scaling |
| **DynamoDB On-Demand** | AWS | NoSQL | Pay-per-request |
| **Cosmos DB Serverless** | Azure | Multi-model | Request-based |

## 🤖 AI/ML Services

### Machine Learning Platforms
| Provider | Service | Capabilities | Use Cases |
|----------|---------|--------------|-----------|
| **AWS** | SageMaker | Full ML lifecycle | Model development |
| **Azure** | Machine Learning | MLOps, AutoML | Enterprise ML |
| **GCP** | AI Platform | Training, prediction | Google's AI expertise |
| **Alibaba** | Machine Learning PAI | End-to-end ML | Asian markets |

### Pre-trained AI Services
| Category | AWS | Azure | GCP |
|----------|-----|-------|-----|
| **Vision** | Rekognition | Computer Vision | Vision API |
| **Speech** | Transcribe, Polly | Speech Services | Speech-to-Text |
| **Language** | Comprehend | Text Analytics | Natural Language |
| **Translation** | Translate | Translator | Translation API |

### Specialized AI
| Service | Provider | Purpose | Use Cases |
|---------|----------|---------|-----------|
| **AWS DeepRacer** | AWS | Reinforcement learning | Education |
| **Azure Bot Service** | Azure | Chatbot development | Customer service |
| **Google AutoML** | GCP | Custom model training | Domain-specific AI |

## 🛠️ DevOps & Management

### CI/CD Services
| Provider | Service | Features | Integration |
|----------|---------|----------|-------------|
| **AWS** | CodePipeline | Full CI/CD pipeline | AWS services |
| **Azure** | DevOps | Boards, repos, pipelines | Microsoft ecosystem |
| **GCP** | Cloud Build | Container-native CI/CD | GCP services |

### Infrastructure Management
| Service | Provider | Purpose | Features |
|---------|----------|---------|----------|
| **AWS CloudFormation** | AWS | Infrastructure as Code | JSON/YAML templates |
| **Azure Resource Manager** | Azure | Resource management | ARM templates |
| **Google Deployment Manager** | GCP | Infrastructure deployment | Python/Jinja2 |

### Monitoring & Logging
| Provider | Service | Type | Features |
|----------|---------|------|----------|
| **AWS** | CloudWatch | Monitoring/Logging | Metrics, alarms, logs |
| **Azure** | Monitor | Observability | Application insights |
| **GCP** | Operations Suite | Monitoring/Logging | Stackdriver successor |

## 🔒 Security Services

### Identity & Access Management
| Provider | Service | Features | Use Cases |
|----------|---------|----------|-----------|
| **AWS** | IAM | Users, roles, policies | Access control |
| **Azure** | Active Directory | Identity management | Enterprise identity |
| **GCP** | Cloud IAM | Resource-level permissions | Fine-grained access |

### Security Monitoring
| Service | Provider | Purpose | Features |
|---------|----------|---------|----------|
| **AWS GuardDuty** | AWS | Threat detection | ML-based detection |
| **Azure Security Center** | Azure | Security posture | Recommendations |
| **Google Security Command Center** | GCP | Security insights | Asset inventory |

### Encryption & Secrets
| Service | Provider | Type | Use Cases |
|---------|----------|------|-----------|
| **AWS KMS** | AWS | Key management | Encryption keys |
| **Azure Key Vault** | Azure | Secrets management | Keys, secrets, certificates |
| **Google Secret Manager** | GCP | Secret storage | API keys, passwords |

## 💰 Cost Optimization

### Cost Management Tools
| Provider | Service | Features |
|----------|---------|----------|
| **AWS** | Cost Explorer | Cost analysis, budgets |
| **Azure** | Cost Management | Spending analysis |
| **GCP** | Billing | Cost breakdown, budgets |

### Cost Optimization Strategies
| Strategy | Description | Savings Potential |
|----------|-------------|-------------------|
| **Reserved Instances** | Commit to usage | 30-70% |
| **Spot Instances** | Use spare capacity | 50-90% |
| **Right-sizing** | Match resources to needs | 10-30% |
| **Auto-scaling** | Scale based on demand | 20-50% |
| **Storage Tiering** | Use appropriate storage class | 30-80% |

## 🎯 Cloud Selection Guide

### By Use Case
| Use Case | Recommended Provider | Reasoning |
|----------|---------------------|-----------|
| **Startup MVP** | AWS/GCP | Free tiers, quick setup |
| **Enterprise** | AWS/Azure | Comprehensive services |
| **.NET Applications** | Azure | Native integration |
| **Data Analytics** | GCP | BigQuery, AI/ML tools |
| **Global Scale** | AWS | Most regions |
| **Cost-Sensitive** | DigitalOcean/Linode | Simple pricing |

### By Team Size
| Team Size | Strategy | Considerations |
|-----------|----------|----------------|
| **Solo (1)** | Single cloud, managed services | Simplicity over optimization |
| **Small (2-10)** | Cloud-native, serverless | Minimize operations |
| **Medium (10-50)** | Multi-service, some optimization | Balance features and cost |
| **Large (50+)** | Multi-cloud, enterprise features | Vendor negotiation power |

### Migration Strategies
| Current State | Target | Approach |
|---------------|--------|----------|
| **On-premises** | Cloud | Lift-and-shift → Optimize |
| **Single cloud** | Multi-cloud | Gradual service migration |
| **Legacy systems** | Modern cloud | Strangler fig pattern |

## 📊 Cloud Trends 2024

### Emerging Services
- **Edge Computing** - Compute closer to users
- **Quantum Computing** - AWS Braket, Azure Quantum
- **Sustainability** - Carbon-neutral cloud services
- **Industry Clouds** - Vertical-specific solutions

### Key Trends
1. **Serverless Adoption** - Function and container-based
2. **Multi-Cloud** - Avoid vendor lock-in
3. **Edge Computing** - 5G and IoT driving demand
4. **AI/ML Integration** - AI in every service
5. **Security Focus** - Zero-trust architectures

## 📚 Learning Resources

### Free Training
- **AWS Training** - Free digital courses
- **Microsoft Learn** - Azure learning paths
- **Google Cloud Training** - Qwiklabs
- **A Cloud Guru** - Free tier available

### Certifications
| Provider | Entry Level | Professional | Expert |
|----------|-------------|--------------|--------|
| **AWS** | Cloud Practitioner | Solutions Architect | Solutions Architect Pro |
| **Azure** | Fundamentals | Administrator | Expert |
| **GCP** | Cloud Digital Leader | Associate | Professional |

### Hands-On Practice
- **AWS Free Tier** - 12 months free services
- **Azure Free Account** - $200 credit + free services
- **GCP Free Tier** - $300 credit + always free
- **Qwiklabs** - Hands-on cloud labs

---

*Cập nhật lần cuối: December 2024*