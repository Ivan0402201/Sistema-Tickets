# 🎫 Sistema de Tickets - Dirección General de Combate al Robo de Vehículos y Transporte

Este proyecto es un **Sistema de Gestión de Tickets** desarrollado para la **Secretaría de Seguridad del Estado de México**, específicamente para la **Dirección General de Combate al Robo de Vehículos y Transporte (DGCRVYT)**.

## 🛠️ Tecnologías Utilizadas

- **HTML5**
- **CSS3**
- **PHP** (mínimo uso)
- **JavaScript (solo si aplica)**
- **SQL Server** (como motor de base de datos)

## 📌 Descripción General

El sistema permite gestionar reportes (tickets) generados por diferentes áreas operativas. Su objetivo principal es organizar y atender fallas técnicas de forma eficiente, permitiendo a cada área generar, consultar y dar seguimiento a sus propios tickets.

## 🧩 Estructura del Sistema

- `index.html`: Página principal con botones de acceso para **Usuario** y **Administrador**.
- `RegistroUser.html`: Registro de usuarios por área con redirección automática según área seleccionada.
- `RegistroAdmi.html`: Acceso para administradores (usuarios: Victor, Isma, Ivan) con validación por correo y contraseña.
- `tickets_analisis.html`, `tickets_investigacion.html`, etc.: Páginas de visualización de tickets por área.
- `formulario.html`: Formulario universal para generar tickets. El área se define según la página de origen.

## 🧾 Categorías de Tickets

1. Servicio de Internet  
2. Equipo de Cómputo  
3. Telefonía  
4. Impresión  
5. Mantenimiento Preventivo  
6. Reubicación de Equipos

## ⚙️ Funcionalidades

- Registro de tickets con folio, nombre, fecha, área, tipo de falla, observaciones y estado.
- Los tickets nuevos se guardan con estado “**Abierto**”.
- Los administradores pueden visualizar y cambiar el estado a “**Cerrado**” cuando la falla se resuelve.
- Redirección automática al área correspondiente tras el inicio de sesión.
- Visualización dinámica de tickets por área.
- Formularios accesibles sin necesidad de volver a seleccionar el área.

## 🔐 Seguridad

- Contraseña única por área.
- Validación de acceso para administradores por correo y contraseña.
- Panel de **Super Administrador** con acceso adicional a funciones especiales (si aplica).

## 🧠 Estructura de la Base de Datos (SQL Server)

Tabla: `tickets`

| Campo         | Tipo             |
|---------------|------------------|
| `id`          | int (PK)         |
| `folio`       | nvarchar(20)     |
| `nombre`      | nvarchar(100)    |
| `fecha`       | date             |
| `area`        | nvarchar(50)     |
| `tipo_falla`  | nvarchar(50)     |
| `observaciones` | nvarchar(max)  |
| `status`      | nvarchar(20)     |

## 📦 Instalación Local

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/Ivan0402201/NOMBRE-DEL-REPO.git
