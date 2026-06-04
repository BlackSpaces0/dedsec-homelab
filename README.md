# 🔐 DedSec Security Lab — HomeLab 2026
> HomeLab personal de ciberseguridad y pentesting | Santo Domingo, RD

## 🖧 Topología de Red

    Internet
        │
    [Router] — x.x.x.x
        │
    [Switch PoE managed]
        ├── ded      x.x.x.xx  (Linux)
        ├── CYBER  x.x.x.xx  (Linux)
        └── len   x.x.x.xx  (Parrot)

## 🖥️ Nodos

| Nodo | Rol | OS |
|---|---|---|
| ded*** | Atacante principal | Linux|
| CYB*** | Servidor de servicios | Linux |
| len*** | Máquina víctima | Parrot|

## 🔧 Servicios instalados

### ded***(Atacante)
- Kali Linux con 600+ herramientas
- Nessus Essentials
- UniFi Network Controller
- Docker

### CY**** (Servidor)
- Apache · MariaDB · PHP
- DVWA (entorno de práctica web)

### len*** (Víctima)
- Servicios de red para práctica
- Docker + Vulhub (158 entornos vulnerables)
- DVWA (segundo objetivo web)

## 🌐 Hardware de red

| Tipo | Modelo (parcial) | Función |
|---|---|---|
| Router ISP | Hua*** HG8*** | Gateway principal |
| Switch PoE | TP-L*** TL***** | Conectividad de nodos |
| Firewall | Ubiq*** USG-*** | Segmentación de red |
| AP WiFi | Ubiq*** nano*** | Cobertura inalámbrica |
| PDU rack | VEN*** HP-*** | Distribución de energía |

## 🖥️ Hardware de cómputo

| Nodo | Fabricante | Función |
|---|---|---|
| ded | Len*** *** | Atacante |
| CYBER | HP *** | Servidor |
| len | Len*** *** | Víctima |

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
