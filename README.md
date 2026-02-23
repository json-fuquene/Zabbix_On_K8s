# Zabbix - Monitoring en Kubernetes

## ¿Qué es Zabbix?

Zabbix es una plataforma de monitoreo empresarial de código abierto diseñada para supervisar la disponibilidad, rendimiento y estado de infraestructura TI. Permite monitorear servidores, redes, aplicaciones, bases de datos, servicios en la nube y entornos contenerizados como Kubernetes, mediante métricas, logs y eventos.

Está orientado a la observabilidad centralizada, alertamiento proactivo y análisis histórico de datos.

---

## Características Principales

### 1. Monitoreo Integral
- Infraestructura (CPU, memoria, disco, red)
- Servicios y aplicaciones
- Contenedores y clústeres Kubernetes
- Bases de datos
- Dispositivos de red (SNMP)
- APIs y endpoints HTTP

### 2. Recolección Flexible de Datos
- Agente Zabbix (activo y pasivo)
- SNMP
- IPMI
- JMX
- HTTP/HTTPS checks
- Webhooks
- Prometheus exporters (integración común en Kubernetes)

### 3. Alertamiento Avanzado
- Triggers basados en umbrales o expresiones lógicas
- Escalamiento automático
- Notificaciones por:
  - Email
  - Webhooks
  - Slack / Teams
  - SMS (mediante integraciones)

### 4. Visualización y Dashboards
- Paneles personalizables
- Gráficas históricas
- Mapas de infraestructura
- Reportes automáticos

### 5. Alta Escalabilidad
- Arquitectura basada en:
  - Zabbix Server
  - Base de datos (MySQL, PostgreSQL, etc.)
  - Proxy distribuido
- Soporta entornos empresariales de gran tamaño

### 6. Integración con Kubernetes
- Monitoreo de:
  - Nodes
  - Pods
  - Containers
  - Métricas del API Server
- Despliegue mediante:
  - Helm Charts
  - Manifiestos YAML
  - Operadores
- Integración con Prometheus para recolección de métricas del clúster

---

## Componentes Principales

- **Zabbix Server**: Motor central de procesamiento.
- **Zabbix Agent**: Recolector de métricas en nodos.
- **Zabbix Proxy**: Recolección distribuida en entornos grandes.
- **Frontend Web**: Interfaz gráfica de administración.
- **Base de Datos**: Almacenamiento histórico de métricas y eventos.

---

## Objetivo de la Implementación en Kubernetes

En este proyecto, Zabbix se implementa en Kubernetes con el propósito de:

- Centralizar el monitoreo del clúster.
- Supervisar cargas de trabajo contenerizadas.
- Detectar fallos de manera proactiva.
- Generar alertas automatizadas.
- Mantener trazabilidad histórica del rendimiento.

---

## Beneficios

- Plataforma madura y estable.
- Open Source y altamente configurable.
- Compatible con entornos híbridos y multi-cloud.
- Escalable y adecuada para producción.
- Amplio soporte comunitario y empresarial.

---

Este README documenta la base conceptual para la implementación de Zabbix en un entorno Kubernetes productivo.