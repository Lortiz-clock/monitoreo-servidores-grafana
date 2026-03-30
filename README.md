# Sistema de Monitoreo de Infraestructura con Nagios Core y Grafana

Este proyecto consiste en el despliegue de una arquitectura de monitoreo profesional para servidores, diseñada para optimizar la visibilidad del rendimiento de hardware en tiempo real. Implementé una solución robusta utilizando virtualización y herramientas de código abierto líderes en la industria.

## 🚀 Arquitectura del Proyecto

La solución se basa en una estructura de capas para garantizar la eficiencia y el bajo consumo de recursos:

1.  **Hipervisor:** Windows Server 2019 (Hyper-V).
2.  **Sistema Operativo del Servidor de Monitoreo:** Rocky Linux (Distribución basada en RHEL) ejecutado en modo *headless* (sin interfaz gráfica) para maximizar el rendimiento.
3.  **Motor de Monitoreo:** Nagios Core, configurado para recibir telemetría mediante agentes en servidores remotos.
4.  **Visualización de Datos:** Grafana, conectado a la base de datos de métricas para la generación de dashboards dinámicos.

## 🛠️ Tecnologías Utilizadas

* **SO:** Rocky Linux, Windows Server 2019.
* **Virtualización:** Hyper-V.
* **Monitoreo:** Nagios Core.
* **Visualización:** Grafana & SQL Queries.
* **Protocolos/Agentes:** NRPE / SNMP.

## 📊 Características Principales

* **Monitoreo en Tiempo Real:** Seguimiento de métricas críticas como uso de CPU, Memoria RAM (Utilizada vs Libre) y Almacenamiento.
* **Optimización de Recursos:** Despliegue en entorno Linux minimalista para reducir el overhead del sistema.
* **Dashboards Personalizados:** Creación de visualizaciones mediante consultas SQL/PromQL para facilitar la toma de decisiones proactiva.

## 📸 Vista Previa del Dashboard

![Dashboard de Monitoreo](URL_DE_TU_IMAGEN_AQUI)

> *Descripción: Panel principal donde se observa el estado de salud de los servidores monitoreados, permitiendo identificar cuellos de botella de manera inmediata.*

## 💡 Retos Técnicos Superados

* Configuración de la comunicación entre agentes y el servidor central a través de diferentes redes virtuales.
* Optimización de la base de datos de Grafana para asegurar la persistencia de datos históricos sin saturar el almacenamiento del servidor Rocky Linux.