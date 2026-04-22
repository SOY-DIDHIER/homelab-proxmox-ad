# 🖥️ Homelab — Proxmox + Windows Server + Active Directory

Infraestructura corporativa virtualizada en entorno doméstico real.  
Objetivo: practicar y documentar configuraciones de nivel empresarial.

---

## 🏗️ Infraestructura del Lab

| Componente | Detalle |
|---|---|
| Hardware | Lenovo M90q G2 |
| CPU | Intel i5-10500T |
| RAM | 32 GB |
| Hipervisor | Proxmox VE |

## 🖥️ Máquinas Virtuales

| VM | Sistema | Rol |
|---|---|---|
| DC01 | Windows Server 2019 | Domain Controller · AD · DNS · DHCP |
| CLIENT01 | Windows 10 | Equipo de usuario unido al dominio |
| LINUX01 | Ubuntu Server | Servidor Linux |

---

## 📋 Proyectos Documentados

### ✅ Active Directory Corporativo
- Dominio: `corp.lab.local`
- Unidades Organizativas: IT · RRHH · Ventas
- Usuarios y grupos por departamento
- GPOs aplicadas por OU

### 🔨 En construcción
- Configuración de File Server con permisos NTFS
- Hardening básico de Windows Server
- Monitorización con herramientas open source
- Backup automatizado

---

## 📬 Contacto

- 💼 [LinkedIn](https://www.linkedin.com/in/didhier-palacios)
- 📧 didhierpalacios@gmail.com
