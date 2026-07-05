# Homelab Infraestructura IT
**Mehboob Subhani** — Técnico de Sistemas Junior

Infraestructura IT completa desplegada en VirtualBox con red segmentada
por zonas (WAN/LAN/DMZ), servicios en Docker, monitorización con Grafana,
Active Directory, seguridad activa con Suricata y automatización con
Bash y Python.

> 🚧 Proyecto en desarrollo activo

## Arquitectura de red
| Zona | Red | Gateway | Propósito |
|------|-----|---------|-----------|
| LAN  | 192.168.1.0/24 | 192.168.1.1 | Red interna corporativa |
| DMZ  | 172.16.0.0/24  | 172.16.0.1  | Servicios públicos |

## Servidores
| VM | Rol | IP | Estado |
|----|-----|----|--------|
| VM1 | OPNsense Firewall | 192.168.1.1 / 172.16.0.1 | ✅ En progreso |
| VM2 | NAS + Monitorización | 192.168.1.10 | ⏳ Pendiente |
| VM3 | Backups | 192.168.1.20 | ⏳ Pendiente |
| VM4 | DMZ Web + IDS | 172.16.0.10 | ⏳ Pendiente |
| VM5 | Active Directory | 192.168.1.30 | ⏳ Pendiente |

## Stack tecnológico
- **Firewall/Red:** OPNsense · Suricata IDS/IPS · VLANs
- **Virtualización:** VirtualBox
- **Servicios:** Docker · Samba · Gitea · Flask · MySQL
- **Monitorización:** Grafana · Prometheus · Loki · Uptime Kuma
- **Directorio:** Active Directory · GPOs · ACLs
- **Automatización:** Bash · Python · cron

## Fases del proyecto
- [x] Fase 1 — Red base y firewall (OPNsense)
- [ ] Fase 2 — Servicios internos (NAS, Gitea, Docker)
- [ ] Fase 3 — Monitorización completa
- [ ] Fase 4 — DMZ y seguridad activa
- [ ] Fase 5 — Active Directory y automatización

## Documentación
- [VM1 — OPNsense](docs/vm1-opnsense.md)
- [VM2 — NAS + Monitorización](docs/vm2-nas-monitorizacion.md)
- [VM3 — Backups](docs/vm3-backups.md)
- [VM4 — DMZ Web](docs/vm4-dmz-web.md)
- [VM5 — Active Directory](docs/vm5-active-directory.md)
