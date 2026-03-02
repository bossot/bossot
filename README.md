# 👋 Hola, sóc en Santi!

🚀 **Platform Engineer** | 🏠 **Homelab Architect** | 🎮 **Gamer & Anime Fan**
📍 Mallorca | 💼 Platform Engineer | 👨‍👩‍👧‍👦 Pare de família

---

## 🏗️ **El Meu Univers Homelab**

El meu homelab està gestionat amb filosofia **GitOps + IaC**, documentat en format [Diátaxis](https://diataxis.fr/) sobre MkDocs.

[![Repositori Homelab](https://img.shields.io/badge/📚-Repositori_Homelab-2ea44f?style=for-the-badge)](https://github.com/ramisclar/tekgarden)

### 🖥️ **Stack de Hardware**
| Component | Especificacions | Funció |
|-----------|----------------|--------|
| **Node Proxmox** | CPU d'alt rendiment, 64GB RAM, emmagatzematge NVMe | Node principal de computació |
| **Servidor NAS** | 64GB RAM, 4×4TB RAID10 | NAS amb 30+ contenidors Docker |
| **VPS al núvol** | Proveïdor europeu | Reverse proxy públic amb Nginx |

### ☸️ **Cluster k3s**
6 nodes (3 control plane + 3 workers) gestionats amb **FluxCD** en mode GitOps pur.
- **VLAN privada** per aïllament del cluster
- **Secrets**: Gestió externa amb password manager
- **Ingress**: Traefik amb terminació TLS

### 🌐 **Serveis Desplegats**
| Servei | Funció | Tecnologia |
|--------|--------|------------|
| 🏠 Home Assistant | Automatització de llar | ESPHome, Zigbee |
| 📸 Galeria de fotos | Gestió personal de fotos | Immich |
| 📰 Lector RSS | Agregació de notícies | Miniflux |
| 🔐 SSO/IdP | Autenticació i autorització | Authentik |
| 📊 Monitorització | Mètriques i visualització | Prometheus+Grafana |
| 🔖 Gestor d'enllaços | Organització de links | Linkding |

### 🌐 **Arquitectura de Xarxa**
**DNS dividit** amb instàncies redundants de Pi-hole:
- Dominis públics → Proxy al núvol → Internet
- Dominis interns → Resolució local directa

**Segmentació per VLANs:**
- **LAN**: Xarxa domèstica
- **SRV**: VLAN de servidors
- **DOCKER**: Xarxa de contenidors
- **DNS**: VLAN de servidors DNS
- **K8S**: VLAN del cluster Kubernetes

### 🔐 **Seguretat - Defensa en Profunditat**
**Arquitectura de seguretat de 3 capes:**
1. **Firewall** - Regles granulars, polítiques restrictives de VPN
2. **Proxy al núvol + Seguretat** - SSO, aprovacions de dispositius, bloqueig geoIP
3. **Reverse Proxy** - Reenviaments d'autenticació, capçaleres de seguretat, limitació de taxa

### 💾 **Estratègia de Backup (3-2-1)**
- **Backups locals** → Sincronització a emmagatzematge al núvol
- **Backups al NAS** → Sincronització a emmagatzematge al núvol
- **Snapshots locals** amb BTRFS
- **Disc extern** setmanal amb air-gap

---

## 🛠️ **Stack Tècnic i Habilitats**

### ☁️ **Núvol i Infraestructura**
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![Proxmox](https://img.shields.io/badge/-Proxmox-E57000?logo=proxmox&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![Ansible](https://img.shields.io/badge/-Ansible-EE0000?logo=ansible&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-623CE4?logo=terraform&logoColor=white)

### 🔧 **Platform Engineering**
![FluxCD](https://img.shields.io/badge/-FluxCD-0D1220?logo=flux&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?logo=github-actions&logoColor=white)
![CI/CD](https://img.shields.io/badge/-CI/CD-FF6C37?logo=jenkins&logoColor=white)
![Monitorització](https://img.shields.io/badge/-Monitorització-F2B820?logo=prometheus&logoColor=white)

### 🏠 **Automatització de Llar**
![Home Assistant](https://img.shields.io/badge/-Home_Assistant-41BDF5?logo=home-assistant&logoColor=white)
![ESPHome](https://img.shields.io/badge/-ESPHome-000000?logo=esphome&logoColor=white)
![Zigbee](https://img.shields.io/badge/-Zigbee-EB5440?logo=zigbee&logoColor=white)

### 💻 **Programació i Scripting**
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?logo=gnu-bash&logoColor=white)
![YAML](https://img.shields.io/badge/-YAML-CB171E?logo=yaml&logoColor=white)

### 🛠️ **Stack Tècnic**
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

## 📊 **Estadístiques de GitHub**

![Estadístiques GitHub](https://github-readme-stats.vercel.app/api?username=bossot&show_icons=true&theme=radical&hide_border=true&count_private=true)

![Llenguatges Principals](https://github-readme-stats.vercel.app/api/top-langs/?username=bossot&layout=compact&theme=radical&hide_border=true)

![Ratxa GitHub](https://streak-stats.demolab.com/?user=bossot&theme=radical&hide_border=true)

---

## 🎯 **Projectes Destacats**

### 🏗️ **[Infraestructura Homelab](https://github.com/ramisclar/tekgarden)**
Homelab complet amb GitOps, documentació Diátaxis i automatització total.

### 🏠 **[Configuracions Home Assistant](https://github.com/ramisclar/home-assistant-config)**
Configuracions d'automatització de llar amb ESPHome, Zigbee i integracions locals.

### 🎮 **[Servidor Minecraft](https://github.com/ramisclar/minecraft-server)**
Servidor Minecraft amb Docker, mods i administració automatitzada.

### 🔐 **[Gestió de Secrets Externs](https://github.com/ramisclar/op-external-secrets)**
Configuració per gestionar secrets de Kubernetes amb gestor de contrasenyes.

### ⚠️ **Millora Contínua**
- Automatització de backups de bases de dades
- Automatització de configuració DNS
- Implementació de stack d'observabilitat de logs
- Millora de monitorització d'infraestructura

---

## 🌟 **Sobre Mi**

- **👨‍💻 Professional**: Platform Engineer especialitzat en infraestructura cloud, Kubernetes i pipelines CI/CD.
- **🧠 Enfocament**: L'estructura, documentació i automatització són fonamentals per a mi.
- **👨‍👩‍👧‍👦 Família**: Visco a Mallorca amb la meva parella i les nostres dues filles.
- **🎮 Aficions**: Karaoke, Minecraft, anime, cuina tècnica al homelab.
- **💡 Filosofia**: Crear infraestructures fiables, documentades i automatitzades.

---

## 📫 **Connecta amb Mi**

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/ramisclar)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white)](https://github.com/bossot)
[![Discord](https://img.shields.io/badge/-Discord-5865F2?logo=discord&logoColor=white)](https://discord.gg/rubiks)
[![Email](https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white)](mailto:santi@ramisclar.cat)

---

*"La millor infraestructura és la que funciona tan bé que ni te n'adones que hi és."* 🚀

**Última actualització**: Març 2026 | **Manteniment**: Community Manager & Tech Assistant
