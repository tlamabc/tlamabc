# 👋 Hi, I'm Dang Thanh Lam

## System Engineer | Data Center & Infrastructure | Monitoring & DevOps

System Engineer specializing in **Enterprise Monitoring, Data Center Infrastructure, Kubernetes, DevOps, and Infrastructure Operations**.

My experience spans infrastructure from **Layer 1 to Layer 7** — from physical servers, racks, power, cabling, sensors, and network infrastructure to virtualization, Kubernetes, monitoring, security, and applications.

---

## 🧑‍💻 About Me

- 💼 **System Engineer at FPT Telecom**
- 📊 **CheckMK_MSP Administrator for FPT Telecom ISP infrastructure**
- 🏢 Focused on **Enterprise Monitoring & Observability**
- 🖥️ Experienced with **Data Center & Bare-metal Infrastructure**
- ☸️ Working with **Kubernetes, GitOps, Docker and Rancher**
- ⚙️ Infrastructure automation with **Ansible & GitLab CI/CD**
- 🔐 Infrastructure security, hardening and access control
- 📡 Network and telemetry infrastructure
- 🏠 Self-hosting and infrastructure experimentation with **Proxmox VE**

---

# 🚀 Core Areas

## 📊 Enterprise Monitoring & Observability

One of my main responsibilities is administering and improving enterprise monitoring infrastructure.

### CheckMK_MSP

I administer **CheckMK_MSP** monitoring infrastructure for the **FPT Telecom ISP environment**, covering monitoring operations and infrastructure observability.

Responsibilities include:

- CheckMK_MSP administration
- Host and service monitoring
- Monitoring infrastructure operations
- SNMP-based monitoring
- Monitoring configuration
- Alerting and incident visibility
- Monitoring integration with infrastructure services
- Polling infrastructure optimization
- Monitoring availability and reliability

The monitoring environment is designed to support large-scale ISP infrastructure and operational requirements.

### Other Monitoring Technologies

- **CheckMK_MSP**
- Cacti
- Prometheus
- ELK Stack
- SNMP
- Metric Exporters
- Custom Telemetry
- Auto-Ticket & Call APIs

---

# ⚙️ Monitoring Architecture & Optimization

Worked on improving the performance and scalability of monitoring infrastructure.

### Async Polling

Refactored legacy polling scripts into **asynchronous active checks** to reduce:

- Zombie processes
- Unnecessary process overhead
- Polling server resource consumption

### Distributed Multi-Poller Architecture

Investigated **Disk Stuck I/O bottlenecks** affecting monitoring workloads.

Re-architected the polling infrastructure into a **distributed Master-Slave / Multi-Poller model** to distribute polling workloads and improve monitoring infrastructure scalability.

```text
                    Monitoring Platform
                           │
                           │
                    ┌──────┴──────┐
                    │   Master    │
                    │  Monitoring │
                    └──────┬──────┘
                           │
             ┌─────────────┼─────────────┐
             │             │             │
             ▼             ▼             ▼
        Multi-Poller  Multi-Poller  Multi-Poller
             │             │             │
             ▼             ▼             ▼
         Network        Servers       Services
          Devices        Hosts        / Apps
```

The objective is to avoid concentrating polling workloads on a single polling node and improve the overall reliability of the monitoring infrastructure.

---

# 🔐 Security & System Hardening

Infrastructure security is another part of my engineering work.

### Monitoring Security

Worked on hardening monitoring platforms including:

- **CheckMK_MSP**
- Cacti
- Web application security
- Access control

Security areas include:

- XSS
- SQL Injection
- Authentication & Access Control
- Server Hardening

---

# 🛡️ WAF & Security Research

## Open-Source WAF with AI Security Analysis

**Graduation Thesis — University of Information Technology (UIT), VNU HCM**

Architected an open-source Web Application Firewall security analysis platform using:

- **BunkerWeb**
- **ModSecurity**
- **OWASP CRS**
- **Ollama**
- Local LLM

The system analyzes security events and provides automated analysis of potential security threats.

### Security Pipeline

```text
                    Incoming Request
                           │
                           ▼
                    ┌─────────────┐
                    │  BunkerWeb  │
                    │     WAF     │
                    └──────┬──────┘
                           │
                           ▼
                    ┌─────────────┐
                    │ ModSecurity │
                    │  + OWASP CRS│
                    └──────┬──────┘
                           │
                           ▼
                    Security Events
                           │
                           ▼
                    ┌─────────────┐
                    │   Ollama    │
                    │   Local LLM │
                    └──────┬──────┘
                           │
                           ▼
                  Security Analysis
```

---

# 🏢 Data Center & Systems

Working with infrastructure from physical hardware to virtualization.

### Data Center Operations

- Bare-metal server operations
- Server rack & relocation
- Hardware sensor management
- Power cabling
- Optical troubleshooting
- Component replacement
- Remote console routing
- ToR networking
- Data center hardware auditing

### Virtualization

- VMware ESXi
- Proxmox VE
- Hardware virtualization

---

# 🌐 Network Infrastructure

Experience with network infrastructure and Data Center network architecture.

### Technologies & Concepts

- L2 / L3 Switching
- ToR Switching
- Spine-Leaf Architecture
- Traditional 3-Tier Architecture
- Network Port Inventory
- Optical troubleshooting
- Console routing

### Academic Research

Simulated and benchmarked:

```text
Spine-Leaf Data Center Architecture
                vs
Traditional 3-Tier Architecture
```

using **GNS3**.

---

# ☸️ Kubernetes & Cloud-Native

Working with containerized infrastructure and GitOps-based application deployment.

### Kubernetes Stack

- Kubernetes
- K3s
- Rancher
- Docker
- Docker Swarm

### GitOps

- ArgoCD
- Helm
- GitLab CI/CD

### Deployment Workflow

```text
        Developer
            │
            ▼
        GitLab Repo
            │
            ▼
       GitLab CI/CD
            │
            ▼
      Container Image
            │
            ▼
       Helm / GitOps
            │
            ▼
          ArgoCD
            │
            ▼
       Kubernetes
            │
            ▼
        Monitoring
```

Deployed applications on Kubernetes using **ArgoCD + Helm following GitOps practices**, with monitoring requirements integrated into application deployment.

---

# ⚙️ Automation & Integration

I use automation to reduce repetitive operational work and improve infrastructure consistency.

### Automation

- Ansible
- GitLab CI/CD
- GitOps
- Automated inventory synchronization
- Monitoring configuration automation
- Network port inventory synchronization

### API Integration

- Ticketing APIs
- Calling APIs
- Monitoring alert integration
- Custom telemetry services

---

# 📡 IoT Telemetry

Developed a Node.js RESTful telemetry ingestion service for real-time IoT packet processing.

### Technology Stack

- Node.js
- REST API
- RabbitMQ
- PostgreSQL
- Hex → JSON packet parsing

### Architecture

```text
IoT Device
    │
    ▼
Telemetry Packet
    │
    ▼
Node.js REST API
    │
    ▼
Packet Parsing
Hex → JSON
    │
    ▼
RabbitMQ
    │
    ▼
PostgreSQL
```

---

# 🚀 DevOps Experience

## Associate DevOps Engineer — iCSP Company

**07/2024 — 08/2025**

Worked with:

- GitLab CI/CD
- Docker
- K3s
- Rancher
- VMware ESXi
- HAProxy
- Ansible
- Data Center infrastructure
- IoT telemetry

### CI/CD Optimization

Built GitLab CI pipelines that reduced deployment time from:

```text
~30 minutes
     │
     ▼
< 5 minutes
```

---

# 🏢 System Engineer Experience

## FPT Telecom

**System Engineer — 09/2025 → Present**

Main areas:

### Observability & Monitoring

- Enterprise monitoring systems
- **CheckMK_MSP administration**
- Cacti
- Prometheus
- ELK Stack
- SNMP
- Metric Exporters
- Custom Telemetry
- Auto-Ticket & Call APIs
- Monitoring architecture optimization

### Automation & Integration

- Network inventory synchronization
- Network port inventory
- Monitoring configuration
- Automated ticketing
- Calling API integration

### Security & Master-Slave

- Monitoring platform hardening
- Access control
- Security analysis
- Polling infrastructure optimization
- Distributed Multi-Poller architecture
- Disk I/O bottleneck investigation

### SLA / OLA Standardization

Worked on standardizing SLA/OLA metrics across infrastructure divisions, including:

- Data Center
- Streaming Services
- NOC / SOC
- Network Backbone

### Hardware & Data Center

- Bare-metal servers
- Server rack operations
- Power cabling
- Hardware sensors
- Component replacement
- VMware ToR networking
- Console routing
- Power / optical troubleshooting

### Kubernetes & GitOps

- Kubernetes application deployment
- ArgoCD
- Helm
- GitOps
- Monitoring requirements for newly deployed services

### Operations & On-call

- 24/7 operations
- High-concurrency streaming service incidents
- Weekly operational reports
- Monitoring and infrastructure incident response

---

# 🏠 Homelab

I maintain a personal infrastructure lab for experimenting with virtualization, networking, self-hosting, and infrastructure operations.

## Hardware

- Proxmox VE
- X99 platform
- Intel Xeon 24-Core
- 32 GB RAM

## Infrastructure

- Hardware virtualization
- L2 / L3 switching
- WiFi integration
- Reverse SSH tunneling
- Remote VPS
- Secure Internet exposure

The homelab is used to experiment with infrastructure concepts before applying them to larger environments.

---

# 🧰 Technical Stack

| Category | Technologies |
|---|---|
| **Monitoring** | **CheckMK_MSP**, Cacti, Prometheus, ELK Stack, SNMP |
| **Observability** | Metric Exporters, Custom Telemetry, Async Polling, Multi-Poller |
| **Data Center** | Bare-metal, ToR, Rack Operations, Power, Optics, Hardware Sensors |
| **Virtualization** | VMware ESXi, Proxmox VE |
| **Containers** | Kubernetes, K3s, Docker, Docker Swarm |
| **GitOps** | ArgoCD, Helm |
| **CI/CD** | GitLab CI/CD |
| **Automation** | Ansible |
| **Networking** | L2/L3, ToR, Spine-Leaf, 3-Tier |
| **Load Balancing** | HAProxy |
| **Messaging** | RabbitMQ |
| **Database** | PostgreSQL, Firebase, Supabase |
| **Security** | BunkerWeb, ModSecurity, OWASP CRS |
| **Security Analysis** | Ollama, Local LLM |
| **Backend** | Node.js, REST API |
| **Development** | Java OOP, Android |
| **Homelab** | Proxmox VE, VMware, Virtualization, L2/L3 |

---

# 🎓 Education

## University of Information Technology (UIT) — VNU HCM

**Bachelor of Science in Information Technology**

**Graduating 2026**

### Graduation Thesis

**Open-Source WAF with AI Security Analysis**

Technologies:

- BunkerWeb
- ModSecurity
- OWASP CRS
- Ollama
- Local LLM

---

## FPT Polytechnic College Da Nang

**Associate Degree in Software Engineering**

**2021 — 2024**

### Capstone Project — Team Lead

Full-stack mobile application using:

- Android
- Firebase
- Supabase

The project included a self-hosted Supabase backend for database management and real-time data synchronization.

---

# 📚 Certification Roadmap

Currently preparing for infrastructure-oriented certifications:

- 🎯 CKA — Certified Kubernetes Administrator
- 🎯 CCNP — Cisco Certified Network Professional
- 🎯 LFCS — Linux Foundation Certified System Administrator

---

# 🗺️ Engineering Focus

My current engineering direction:

```text
Software Development
        │
        ▼
     DevOps
        │
        ▼
 Infrastructure
        │
        ├───────────────┐
        ▼               ▼
 Data Center       Kubernetes
        │               │
        └───────┬───────┘
                ▼
        Observability
                │
                ▼
       Enterprise Systems
                │
                ▼
       Reliable Infrastructure
```

I'm particularly interested in building and operating infrastructure that is:

- **Observable**
- **Automated**
- **Scalable**
- **Secure**
- **Reliable**

---

# 📫 Contact

📧 **Email:** dangthanhlam1312@gmail.com

🔗 **LinkedIn:** linkedin.com/in/tlamabe

---

> **Infrastructure is not just about running servers.
> It's about building systems that remain observable, scalable, secure, and reliable under real operational conditions.**
