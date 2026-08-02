---
title: <Arquitectura Cloud>
id: ARC-CLD-130
version: 1.0
status: Draft
owner: Arquetipo Digital
category: Architecture
type: Cloud Architecture
domain: Cloud
framework: ARCHE
classification: Infrastructure
cloud_provider: <Azure | AWS | GCP | MultiCloud | Híbrido>
authors:
  - <Autor>
reviewers:
  - <Revisor>
approvers:
  - <Aprobador>
created: YYYY-MM-DD
last_updated: YYYY-MM-DD
next_review: YYYY-MM-DD
references:
  - ARC-EA-120 Enterprise Architecture
  - ARC-SOL-100 Solution Architecture
  - ARC-SW-110 Software Architecture
  - ADS-003 Quality Attribute Scenarios
  - ADS-004 Architecture Decision Standard
tags:
  - cloud
  - architecture
---

# Arquitectura Cloud

> La nube no es una arquitectura.
>
> Es una plataforma para materializar una arquitectura.

---

# Resumen Ejecutivo

Describir:

- necesidad de negocio;
- objetivos cloud;
- beneficios esperados;
- riesgos principales;
- estrategia de adopción.

---

# Información General

| Campo | Valor |
|--------|-------|
| Proyecto | |
| Organización | |
| Cloud Provider | |
| Región Principal | |
| Arquitecto Cloud | |
| Estado | |

---

# Contexto

## Problema

¿Qué necesidad impulsa el uso de la nube?

---

## Objetivos

### Negocio

-

### Técnicos

-

### Operacionales

-

---

# Estrategia Cloud

Seleccionar la estrategia.

- Cloud First
- Hybrid Cloud
- MultiCloud
- Cloud Native
- Lift & Shift
- Replatform
- Refactor
- Replace
- Retire
- Retain

Justificar la decisión.

---

# Requisitos No Funcionales

Priorizar.

| Requisito | Prioridad |
|-----------|-----------|
| Disponibilidad | |
| Escalabilidad | |
| Seguridad | |
| Observabilidad | |
| Recuperación | |

---

# Arquitectura General

## Vista Conceptual

```text
Usuarios

↓

Canales

↓

Servicios Cloud

↓

Datos

↓

Integraciones
```

---

## Arquitectura Lógica

Agregar diagrama.

---

## Arquitectura Física

Agregar diagrama.

---

# Landing Zone

Documentar.

- Suscripciones
- Cuentas
- Tenants
- Resource Groups
- Organización
- Naming Convention

---

# Networking

Documentar.

- VNet / VPC
- Subredes
- DNS
- Balanceadores
- Firewall
- VPN
- ExpressRoute / Direct Connect
- Peering

Agregar diagrama.

---

# Computación

Documentar.

| Servicio | Propósito |
|-----------|-----------|
| Kubernetes | |
| App Service | |
| VM | |
| Functions | |
| Containers | |

---

# Almacenamiento

| Servicio | Uso |
|-----------|-----|
| Blob | |
| Files | |
| Object Storage | |

---

# Datos

Documentar.

- SQL
- NoSQL
- Cache
- Data Lake
- Backup
- Replicación

---

# Integración

Documentar.

- API Gateway
- Service Bus
- Event Hub
- Kafka
- Pub/Sub

---

# Seguridad

Documentar.

## IAM

Roles.

Permisos.

Identidades.

---

## Secretos

- Key Vault
- Secrets Manager

---

## Cifrado

En tránsito.

En reposo.

---

## Cumplimiento

- ISO
- SOC
- PCI
- HIPAA
- GDPR
- Normativa local

---

# Observabilidad

Documentar.

- Logs
- Métricas
- Tracing
- Alertas
- Dashboards

Herramientas.

- Azure Monitor
- CloudWatch
- Prometheus
- Grafana
- New Relic

---

# Alta Disponibilidad

Documentar.

- Availability Zones
- Regiones
- Replicación
- Balanceo
- Failover

---

# Recuperación

Definir.

| Objetivo | Valor |
|----------|-------|
| RPO | |
| RTO | |

Describir estrategia de Disaster Recovery.

---

# Costos

## Modelo de Costos

CAPEX

OPEX

Pay as you Go

Reserved

Savings Plan

---

## Estimación

| Servicio | Costo |
|-----------|--------|
| Servicio | |

---

## Optimización

- Auto Scaling
- Rightsizing
- Reserved Instances
- Lifecycle Policies

---

# DevOps

Documentar.

- CI
- CD
- Infraestructura como Código
- GitOps
- Automatización

Herramientas.

- GitHub Actions
- Azure DevOps
- Terraform
- Bicep
- Pulumi

---

# Gobierno Cloud

Documentar.

- Políticas
- Tags
- Naming
- Cost Center
- Compliance

---

# Riesgos

| Riesgo | Mitigación |
|----------|------------|
| Riesgo | |

---

# ADR Relacionados

Referenciar decisiones cloud.

---

# Checklist

## Arquitectura

- [ ] Landing Zone definida
- [ ] Networking documentado
- [ ] Seguridad diseñada

---

## Operación

- [ ] Monitoreo
- [ ] Alertas
- [ ] Backup
- [ ] DR

---

## Gobernanza

- [ ] Políticas
- [ ] Costos
- [ ] Compliance

---

# Documentos Relacionados

- Enterprise Architecture
- Solution Architecture
- Software Architecture
- Security Architecture
- Deployment Architecture
- ADR

---

# Historial

| Versión | Fecha | Descripción |
|----------|------|-------------|
| 1.0 | YYYY-MM-DD | Primera versión |

---

# Aprobaciones

| Rol | Responsable | Fecha |
|------|-------------|------|
| Cloud Architect | | |
| Security Architect | | |
| CIO | | |

---

# Declaración Final

La Arquitectura Cloud define cómo una organización utiliza los servicios de nube para soportar sus capacidades de negocio de forma segura, escalable y sostenible.

Su propósito no es describir únicamente recursos de infraestructura, sino establecer un modelo operativo que permita evolucionar la plataforma de manera gobernada, optimizando costos, resiliencia y velocidad de entrega.

---

> **La nube no aporta valor por sí sola.**
>
> **El valor aparece cuando la arquitectura aprovecha correctamente sus capacidades.**

---

© Arquetipo Digital
