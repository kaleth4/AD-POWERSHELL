# Sysadmin Automation Tool (PowerShell) 🛠️

![PowerShell](https://img.shields.io/badge/PowerShell-5.1+-blue.svg?style=flat&logo=powershell)

Este proyecto está diseñado para automatizar las funciones críticas de un **Administrador de Sistemas (Sysadmin)** mediante PowerShell. Su objetivo es centralizar tareas de configuración de red, gestión de identidades y auditoría de seguridad en una única herramienta ejecutable, ahorrando tiempo y reduciendo errores manuales.

---

## 🚀 Descripción

Este script de PowerShell funciona como una **navaja suiza** para Administradores de Sistemas, permitiendo gestionar infraestructuras Windows, realizar auditorías de red y automatizar configuraciones básicas desde una consola centralizada.

---

## 📌 Funcionalidades

El script incluye un **menú interactivo** con las siguientes capacidades:

### 1️⃣ **Gestión de Identidades (Active Directory)**
- **Instalación:** Configuración automática del rol de **AD DS** y promoción de **Domain Controllers**.
- **Gestión:** Creación de usuarios, grupos y **Unidades Organizativas (OU)**.

### 2️⃣ **Infraestructura de Red (DHCP)**
- Instalación del rol de **Servidor DHCP**.
- Configuración de ámbitos (scopes), exclusiones y tiempos de concesión.
- Autorización del servidor en el dominio.

### 3️⃣ **Auditoría y Pentesting (Networking)**
- **Escaneo de Red:** Identificación de hosts activos mediante **ICMP/ARP**.
- **Escaneo de Puertos:** Verificación de puertos críticos abiertos (80, 443, 445, 3389, etc.) para evaluar la superficie de exposición.
- **Conteo de Equipos:** Reporte rápido de cuántos dispositivos responden en un segmento de red específico.

### 4️⃣ **Tareas de Mantenimiento Básico**
- Cambio de nombre del equipo (Hostname).
- Configuración de direcciones **IP estáticas** y **DNS**.
- Unión a dominios de forma automatizada.

---

## ⚙️ Requisitos

| Requisito | Detalle |
|-----------|---------|
| **Sistema Operativo** | Windows Server 2016 o superior (algunas funciones requieren edición Server). |
| **Privilegios** | Ejecutar PowerShell como **Administrador**. |
| **Política de Ejecución** | `Set-ExecutionPolicy RemoteSigned`. |

---

## 🛠️ Instalación y Uso

1. **Clona el repositorio** o descarga el archivo `.ps1`:
   ```powershell
   git clone https://github.com/tu-usuario/SysadminAutomationTool.git
   ```

2. **Ejecuta el script** (como Administrador):
   ```powershell
   .\SysadminTool.ps1
   ```

⚠️ **Advertencia**
Las funciones de **Escaneo de Puertos** están orientadas a la auditoría de seguridad. **Asegúrate de tener autorización** antes de escanear redes que no te pertenecen.

---

## 📜 Licencia

Este proyecto se distribuye bajo la licencia **[MIT](https://opensource.org/licenses/MIT)**. Consulta el archivo `LICENSE` para más detalles.

---

🔹 **¿Problemas o sugerencias?** Abre un *issue* en el repositorio o envía un *pull request*.
