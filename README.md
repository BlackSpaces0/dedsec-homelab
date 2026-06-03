# 🔐 DedSec Security Lab — HomeLab 2026
> HomeLab personal de ciberseguridad y pentesting | Santo Domingo, RD

## 🖧 Topología de Red

    Internet
        │
    [Router] — x.x.x.x
        │
    [Switch PoE managed]
        ├── dedsec      x.x.x.xx  (Kali Linux 2026)
        ├── CYBER-CORE  x.x.x.xx  (Linux)
        └── lenovosec   x.x.x.xx  (Parrot OS 7.2)

## 🖥️ Nodos

| Nodo | Rol | OS |
|---|---|---|
| dedsec | Atacante principal | Kali Linux 2026 |
| CYBER-CORE | Servidor de servicios | Linux |
| lenovosec | Máquina víctima | Parrot OS 7.2 |

## 🔧 Servicios instalados

### dedsec (Atacante)
- Kali Linux 2026 con 600+ herramientas
- Nessus Essentials
- UniFi Network Controller
- Docker

### CYBER-CORE (Servidor)
- Apache · MariaDB · PHP
- DVWA (entorno de práctica web)

### lenovosec (Víctima)
- Servicios de red para práctica
- Docker + Vulhub (158 entornos vulnerables)
- DVWA (segundo objetivo web)

## 🌐 Hardware de red

| Tipo | Modelo (parcial) | Función |
|---|---|---|
| Router ISP | Hua*** HG8*** | Gateway principal |
| Switch PoE | TP-L*** TL-SG3*** | Conectividad de nodos |
| Firewall | Ubiq*** USG-*** | Segmentación de red |
| AP WiFi | Ubiq*** nano*** | Cobertura inalámbrica |
| PDU rack | VEN*** HP-*** | Distribución de energía |

## 🖥️ Hardware de cómputo

| Nodo | Fabricante | Función |
|---|---|---|
| dedsec | Len*** M9*** | Atacante |
| CYBER-CORE | HP T4*** | Servidor |
| lenovosec | Len*** M72*** | Víctima |

## 📊 Progreso

- [x] Infraestructura base — 3 nodos en red
- [x] SSH entre todos los nodos
- [x] IPs estáticas configuradas
- [x] DVWA en servidor y víctima
- [x] Nessus Essentials operativo
- [x] UniFi Network Controller activo
- [x] Docker + Vulhub instalado
- [x] GitHub documentado
- [ ] SQL Injection en DVWA
- [ ] XSS en DVWA
- [ ] Fuerza bruta con Hydra
- [ ] Writeups de prácticas

## 🛠️ Stack tecnológico

- **Ataque:** Kali Linux · Nessus · Metasploit · Burp Suite · Hydra
- **Defensa:** UniFi · Firewall · VLAN (planificado)
- **Práctica:** DVWA · Vulhub · 158 CVEs disponibles

## 👤 Autor
Enmanuel Rodriguez — BlackSpaces0
