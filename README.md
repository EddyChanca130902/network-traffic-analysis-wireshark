# 🦈 Análisis de Tráfico de Red y Auditoría DNS (Wireshark)

Laboratorio práctico de visibilidad y análisis de tráfico de red utilizando **Wireshark** sobre sistemas operativos **Linux Mint**, enfocado en la comprensión de protocolos de red y análisis de peticiones DNS.

---

## 🛠️ Tecnologías y Entorno
* **Sistema Operativo:** Linux Mint (`wlo1` como interfaz de red física).
* **Herramienta de Análisis:** Wireshark.
* **Herramientas de Red:** Terminal Linux, `ip link show`, `nslookup`.
* **Conceptos Clave:** Permisos a nivel de kernel, captura de paquetes en tiempo real, filtrado de protocolos y análisis de tráfico perimetral.

---

## 🔍 Desarrollo del Laboratorio

1. **Configuración de Permisos y Kernel:**
   * Resolución de restricciones de acceso a las interfaces físicas de red mediante la integración de usuarios a grupos de seguridad y uso de `newgrp wireshark` para refrescar los privilegios de sesión.
   * Identificación de la interfaz inalámbrica real (`wlo1`) utilizando comandos de red del sistema (`ip link show`).

2. **Captura y Filtrado de Tráfico (DNS):**
   * Inicio de la captura de paquetes en la interfaz física seleccionada.
   * Aplicación de filtros de visualización (`dns`) para aislar las consultas y respuestas de resolución de nombres de dominio.
   * Generación de tráfico controlado mediante pruebas de consulta en terminal (`nslookup google.com`).

---

## 💡 Reflexión y Enfoque Profesional
*Siguiendo la analogía de la ciberseguridad defensiva:* Las herramientas de análisis de tráfico como Wireshark son instrumentos legítimos de diagnóstico y visibilidad (*"un cuchillo para untar mantequilla"*). Sin embargo, debido a su capacidad para inspeccionar datos en tránsito, su uso exige un rigor ético absoluto y un manejo profesional orientado al Blue Team. La tecnología es neutral; la responsabilidad y la ética la define el analista.

---
## 📂 Contenido del Repositorio
* `README.md`: Documentación técnica del laboratorio.

