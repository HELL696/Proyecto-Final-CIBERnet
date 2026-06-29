# WandL - Sistema de Gestión de Restaurantes & Infraestructura de Red Segura

Este proyecto fue desarrollado para la materia de **Taller de Programación 1**. Integra un sistema completo de gestión de inventarios y compras para restaurantes con una topología de red local emulada y protegida mediante políticas estrictas de seguridad perimetral.

---

##  Características del Proyecto

### Software (Full-Stack)
* **Backend:** Desarrollado con **FastAPI** (Python), aprovechando su alto rendimiento asíncrono y validación nativa de datos mediante **Pydantic**.
* **Frontend:** Construido en **React**, implementando componentes dinámicos, consumo de APIs mediante **Axios** y un diseño limpio y responsivo con **Bulma CSS**.
* **Módulo Principal:** Gestión de **Insumos Adquiridos** que permite registrar y auditar de forma exacta el Nombre, Precio Unitario y Cantidad de los productos en stock, eliminando el error manual en la administración del restaurante.

### Infraestructura de Red
* **Core:** Emulado en **GNS3** utilizando un Router Cisco 3725 (IOS Real).
* **Segmentación de Red:** Implementación de subredeo lógico optimizado:
  * Subred `/25` destinada al Pool de Clientes y usuarios del cibernet (`192.168.100.0/25`).
  * Subred `/30` de alta seguridad para la PC de Administración y Caja (`192.168.100.128/30`).
* **Firewall Perimetral:** Configuración de una Lista de Control de Acceso (ACL 101) Extendida para mitigar riesgos e intrusiones, aplicando un flujo asimétrico de tráfico ICMP y bloqueo de contenido web no autorizado en la interfaz local.

---

## Arquitectura y Tecnologías

* **Simulación de Red:** GNS3, Cisco IOS.
* **Protocolos & Seguridad:** IPv4 Subnetting, ICMP, ACLs extendidas.

---

## Autores
* Bernardo (Desarrollo Frontend & Redes)
* Laura (Infraestructura de Red)
* Willy (Desarrollo Backend & Redes)
## Video
*https://youtu.be/MgLsadzEYkY
## Documento
https://github.com/HELL696/Proyecto-Final-CIBERnet/blob/main/Red%20estructurada.pdf
