# 👋 Hola, sóc en Santi! 

🚀 **Platform Engineer** | 🏠 **Homelab Architect** | 🎮 **Gamer & Anime Fan**  
📍 Mallorca, Spain | 💼 Platform Engineer | 👨‍👩‍👧‍👦 Family Man

---

## 🏗️ **My Homelab Universe**

El meu homelab està gestionat amb filosofia **GitOps + IaC**, documentat en format [Diátaxis](https://diataxis.fr/) sobre MkDocs.

[![Homelab Repo](https://img.shields.io/badge/📚-Homelab_Repository-2ea44f?style=for-the-badge)](https://github.com/ramisclar/tekgarden)

### 🖥️ **Hardware Stack**
| Component | Especificacions | Funció |
|-----------|----------------|--------|
| **Proxmox Node** | High-performance CPU, 64GB RAM, NVMe storage | Main compute node |
| **NAS Server** | 64GB RAM, 4×4TB RAID10 | NAS with 30+ Docker containers |
| **Cloud VPS** | European provider | Public reverse proxy with Nginx |

### ☸️ **k3s Cluster**
6 nodes (3 control plane + 3 workers) gestionats amb **FluxCD** en mode GitOps pur.
- **Private VLAN** for cluster isolation
- **Secrets**: External Secrets with password manager
- **Ingress**: Traefik with TLS termination

### 🌐 **Services Deployed**
| Servei | Funció | Tecnologia |
|--------|--------|------------|
| 🏠 Home Assistant | Home automation | ESPHome, Zigbee |
| 📸 Photo Gallery | Personal photo management | Immich |
| 📰 RSS Reader | News aggregation | Miniflux |
| 🔐 SSO/IdP | Authentication & authorization | Authentik |
| 📊 Monitoring | Metrics & visualization | Prometheus+Grafana |
| 🔖 Bookmark Manager | Link organization | Linkding |

### 🌐 **Network Architecture**
**Split DNS** with redundant Pi-hole instances:
- Public domains → Cloud proxy → Internet
- Internal domains → Direct local resolution

**VLAN Segmentation:**
- **LAN**: Home network
- **SRV**: Server VLAN
- **DOCKER**: Container network
- **DNS**: DNS servers VLAN
- **K8S**: Kubernetes cluster VLAN

### 🔐 **Security - Defense in Depth**
**3-layer security architecture:**
1. **Firewall** - Granular rules, restrictive VPN policies
2. **Cloud Proxy + Security** - SSO, device approvals, geoIP blocking
3. **Reverse Proxy** - Authentication forwarding, security headers, rate limiting

### 💾 **Backup Strategy (3-2-1)**
- **Local backups** → Sync to cloud storage
- **NAS backups** → Sync to cloud storage
- **Local snapshots** with BTRFS
- **External drive** weekly air-gap backups

---

## 🛠️ **Tech Stack & Skills**

### ☁️ **Cloud & Infrastructure**
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Proxmox](https://img.shields.io/badge/-Proxmox-E57000?logo=proxmox&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![Ansible](https://img.shields.io/badge/-Ansible-EE0000?logo=ansible&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-623CE4?logo=terraform&logoColor=white)

### 🔧 **Platform Engineering**
![FluxCD](https://img.shields.io/badge/-FluxCD-0D1220?logo=flux&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?logo=github-actions&logoColor=white)
![CI/CD](https://img.shields.io/badge/-CI/CD-FF6C37?logo=jenkins&logoColor=white)
![Monitoring](https://img.shields.io/badge/-Monitoring-F2B820?logo=prometheus&logoColor=white)

### 🏠 **Home Automation**
![Home Assistant](https://img.shields.io/badge/-Home_Assistant-41BDF5?logo=home-assistant&logoColor=white)
![ESPHome](https://img.shields.io/badge/-ESPHome-000000?logo=esphome&logoColor=white)
![Zigbee](https://img.shields.io/badge/-Zigbee-EB5440?logo=zigbee&logoColor=white)

### 💻 **Programming & Scripting**
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?logo=gnu-bash&logoColor=white)
![YAML](https://img.shields.io/badge/-YAML-CB171E?logo=yaml&logoColor=white)

### 🛠️ **Technical Stack**
**Domina:**
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![k3s](https://img.shields.io/badge/-k3s-FFC66D?logo=kubernetes&logoColor=black)
![FluxCD](https://img.shields.io/badge/-FluxCD-0D1220?logo=flux&logoColor=white)
![Ansible](https://img.shields.io/badge/-Ansible-EE0000?logo=ansible&logoColor=white)
![OpenTofu](https://img.shields.io/badge/-OpenTofu-7B42BC?logo=opentofu&logoColor=white)
![Proxmox](https://img.shields.io/badge/-Proxmox-E57000?logo=proxmox&logoColor=white)
![pfSense](https://img.shields.io/badge/-pfSense-212121?logo=pfsense&logoColor=white)
![Traefik](https://img.shields.io/badge/-Traefik-24A1C1?logo=traefikproxy&logoColor=white)
![Authentik](https://img.shields.io/badge/-Authentik-0D1220?logo=authentik&logoColor=white)

**Aprenent activament:**
![Loki](https://img.shields.io/badge/-Loki-F7B93E?logo=grafana-loki&logoColor=black)
![Grafana Alloy](https://img.shields.io/badge/-Grafana_Alloy-F46800?logo=grafana&logoColor=white)
![kube-prometheus](https://img.shields.io/badge/-kube--prometheus-F2B820?logo=prometheus&logoColor=white)

---

## 📊 **GitHub Stats**

![GitHub stats](https://github-readme-stats.vercel.app/api?username=ramisclar&show_icons=true&theme=radical&hide_border=true&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=ramisclar&layout=compact&theme=radical&hide_border=true)

![GitHub Streak](https://streak-stats.demolab.com/?user=ramisclar&theme=radical&hide_border=true)

---

## 🎯 **Featured Projects**

### 🏗️ **[Homelab Infrastructure](https://github.com/ramisclar/tekgarden)**
Complete homelab with GitOps, Diátaxis documentation and full automation.

### 🏠 **[Home Assistant Configurations](https://github.com/ramisclar/home-assistant-config)**
Home automation configurations with ESPHome, Zigbee and local integrations.

### 🎮 **[Minecraft Server](https://github.com/ramisclar/minecraft-server)**
Minecraft server with Docker, mods and automated administration.

### 🔐 **[External Secrets Management](https://github.com/ramisclar/op-external-secrets)**
Configuration for managing Kubernetes secrets with password manager.

### ⚠️ **Continuous Improvement**
- Database backup automation
- DNS configuration automation  
- Log observability stack implementation
- Infrastructure monitoring enhancement

---

## 🌟 **About Me**

- **👨‍💻 Professional**: Platform Engineer specialized in cloud infrastructure, Kubernetes and CI/CD pipelines.
- **🧠 Neurodivergent**: Adult ASD - structure, documentation and automation aren't optional, it's how I think.
- **👨‍👩‍👧‍👦 Family**: Living in Mallorca with my partner and our two daughters.
- **🎮 Hobbies**: Karaoke, Minecraft, anime, technical cooking in the homelab.
- **🏴 Values**: Digital sovereignty, open source, anti-BigTech, feminism.

---

## 📫 **Connect With Me**

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/ramisclar)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white)](https://github.com/ramisclar)
[![Discord](https://img.shields.io/badge/-Discord-5865F2?logo=discord&logoColor=white)](https://discord.gg/rubiks)
[![Email](https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white)](mailto:santi@ramisclar.cat)

---

*"The best infrastructure is the one that works so well you don't even notice it's there."* 🚀

**Last update**: March 2026 | **Maintenance**: Community Manager & Tech Assistant