# 🔐 DedSec Security Lab — HomeLab 2026
> HomeLab personal de ciberseguridad y pentesting | Santo Domingo, RD

## 🖧 Topología de Red — 10.0.0.0/24

    Internet
        │
    [Router Huawei HG8145V5] — 10.0.0.1
        │
    [TP-Link TL-SG3424P] — Switch PoE 24p
        ├── dedsec      10.0.0.31  (Kali Linux 2026)
        ├── CYBER-CORE  10.0.0.33  (Linux Lite)
        └── lenovosec   10.0.0.32  (Parrot OS 7.2)

## 🖥️ Nodos

| Nodo | Hardware | OS | IP | Rol |
|---|---|---|---|---|
| dedsec | Lenovo M900 SFF · i5-6500 · 20GB | Kali Linux 2026 | 10.0.0.31 | Atacante |
| CYBER-CORE | HP T430 Thin Client | Linux Lite | 10.0.0.33 | Servidor |
| lenovosec | Lenovo M72e Tiny | Parrot OS 7.2 | 10.0.0.32 | Víctima |

## 🔧 Servicios instalados

### dedsec (Atacante)
- Kali Linux 2026 con 600+ herramientas
- Nessus Essentials
- UniFi Network Controller
- Docker

### CYBER-CORE (Servidor)
- Apache 2.4 · MariaDB · PHP 8.3
- DVWA — http://10.0.0.33/DVWA
- SSH puerto 22

### lenovosec (Víctima)
- Apache · MariaDB · PHP 8.4
- DVWA — http://10.0.0.32/DVWA
- vsftpd FTP puerto 21
- Samba SMB puertos 139/445
- Telnet puerto 23
- Docker + Vulhub 158 entornos vulnerables

## 🌐 Hardware de red

| Equipo | Función |
|---|---|
| Huawei HG8145V5 | Router/Gateway |
| TP-Link TL-SG3424P | Switch PoE 24p managed |
| Ubiquiti USG-3P | Firewall (en camino) |
| Ubiquiti nanoHD | AP WiFi 5 Wave 2 (en camino) |
| PDU VENLOGIC HP-1U | Distribución de energía |

## 🔑 Conexiones SSH

    ssh sysadmoin@10.0.0.33   # dedsec → CYBER-CORE
    ssh lenovosec@10.0.0.32   # dedsec → lenovosec

## 🛠️ Comandos clave

    # Escaneo nmap
    nmap -sV -sC -A -p- 10.0.0.33
    nmap -sV -sC -A -p- -Pn 10.0.0.32

    # Nikto
    nikto -h 10.0.0.33

    # Red completa
    nmap -sn 10.0.0.0/24

    # Vulhub
    cd ~/vulhub/<app>/<cve> && docker-compose up -d

## 📊 Progreso

- [x] Infraestructura base 3 nodos en red
- [x] SSH entre todos los nodos
- [x] IPs estáticas fijadas
- [x] DVWA en CYBER-CORE y lenovosec
- [x] Nessus Essentials en dedsec
- [x] UniFi Network Controller en dedsec
- [x] Docker + Vulhub en lenovosec
- [ ] SQL Injection en DVWA
- [ ] XSS en DVWA
- [ ] Fuerza bruta con Hydra
- [ ] Writeups de prácticas

## 👤 Autor
Enmanuel Rodriguez — BlackSpaces0
