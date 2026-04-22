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
| Hipervisor | Proxmox VE 9.1 |

## 🖥️ Máquinas Virtuales

| VM | Sistema | Rol |
|---|---|---|
| DC01 | Windows Server 2019 | Domain Controller · AD · DNS · DHCP |
| CLIENT01 | Windows 10 | Equipo de usuario unido al dominio |
| LINUX01 | Ubuntu Server | Servidor Linux |

---

## 📋 Active Directory Corporativo

Dominio: `empresa.local`  
Controlador de dominio: `DC01.empresa.local`

### Estructura de OUs

![Estructura AD](todas%20OUs.png)

### Usuarios por departamento

| OU | Usuarios |
|---|---|
| IT | carlos.garcia · ana.martinez · pedro.sanchez |
| RRHH | laura.fernandez · miguel.torres · sofia.romero |
| Ventas | javier.lopez · carmen.diaz · roberto.jimenez |
| Dirección | antonio.morales |

![Usuarios IT](usuarios%20OU-IT.png)
![Usuarios RRHH](usuarios%20OU-RRHH.png)
![Usuarios Ventas](usuarios%20OU-Ventas.png)
![Usuarios Dirección](usuario%20OU-direccion.png)

---

## ⚙️ GPOs Corporativas Implementadas

| GPO | Función |
|---|---|
| GPO-Fondo-Corporativo | Fondo de pantalla corporativo bloqueado |
| GPO-Bloqueo-USB | Bloqueo de lectura y escritura en USB |
| GPO-Politica-Contrasenas | Contraseñas mínimo 8 caracteres · complejidad · historial |

![GPOs](todas%20las%20GPOs.png)

---

## 🔨 En construcción

- File Server con permisos NTFS
- Hardening básico de Windows Server
- Monitorización con herramientas open source
- Backup automatizado
- Unir cliente Windows 10 al dominio

---

## 📬 Contacto

- 💼 [LinkedIn](https://www.linkedin.com/in/didhier-palacios)
- 📧 didhierpalacios@gmail.com
