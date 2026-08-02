---
title: <Arquitectura de Observabilidad>
id: ARC-OBS-190
version: 1.0
status: Draft
owner: Arquetipo Digital
category: Architecture
type: Observability Architecture
domain: Observability
framework: ARCHE
classification: Cross-Cutting
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
  - ARC-SOL-100 Solution Architecture
  - ARC-SW-110 Software Architecture
  - ARC-DEP-170 Deployment Architecture
  - ARC-SEC-180 Security Architecture
  - ADS-003 Quality Attribute Scenarios
tags:
  - observability
  - monitoring
  - sre
---

# Arquitectura de Observabilidad

> No se puede operar correctamente un sistema que no puede comprenderse.

La observabilidad permite entender el comportamiento interno de una solución a partir de la evidencia que produce durante su ejecución.

Su propósito es reducir la incertidumbre operacional y facilitar la toma de decisiones.

---

# Resumen Ejecutivo

Describir:

- objetivos de observabilidad;
- riesgos operacionales;
- capacidades de monitoreo;
- beneficios esperados;
- estrategia de instrumentación.

---

# Información General

| Campo | Valor |
|--------|-------|
| Proyecto | |
| Arquitecto | |
| SRE | |
| Plataforma | |
| Estado | |
| Versión | |

---

# Contexto

## Problema

¿Qué desafíos operacionales pretende resolver esta arquitectura?

---

## Objetivos

### Negocio

-

### Operacionales

-

### Técnicos

-

---

# Principios de Observabilidad

Aplicar los principios utilizados.

Ejemplo.

- Observability by Design
- Telemetry First
- Everything as Data
- Correlation First
- Automation First
- Shift Left Observability

Explicar cómo se aplican.

---

# Preguntas Operacionales

La arquitectura debe responder preguntas como:

- ¿Está disponible el servicio?
- ¿Qué usuario presenta problemas?
- ¿Cuál fue el tiempo de respuesta?
- ¿Qué dependencia está degradada?
- ¿Qué versión produjo el incidente?
- ¿Dónde comenzó la falla?
- ¿Cuál fue el impacto en el negocio?

---

# Arquitectura General

Agregar diagrama.

```text
Aplicación

↓

Instrumentación

↓

Collector

↓

Plataforma Observabilidad

↓

Dashboards

↓

Alertas

↓

Respuesta
```

---

# Señales de Observabilidad

## Logs

Documentar.

- estructura;
- formato;
- correlación;
- retención.

---

## Métricas

Documentar.

- negocio;
- aplicación;
- infraestructura.

---

## Trazabilidad Distribuida

Documentar.

- Trace ID;
- Span ID;
- propagación de contexto;
- correlación.

---

## Eventos

Documentar eventos relevantes.

---

# Instrumentación

Definir estrategia.

- OpenTelemetry
- SDKs
- Agentes
- Instrumentación automática
- Instrumentación manual

---

# Catálogo de Métricas

| Métrica | Tipo | Objetivo |
|----------|------|----------|
| Latencia | Técnica | |
| Throughput | Técnica | |
| Errores | Técnica | |
| Conversión | Negocio | |
| Consentimientos | Negocio | |

Clasificar las métricas por dominio.

---

# Indicadores (KPIs)

| Indicador | Objetivo |
|-----------|----------|
| Disponibilidad | |
| Tiempo Medio de Recuperación (MTTR) | |
| Tiempo Medio entre Fallas (MTBF) | |
| Tiempo de Respuesta | |
| Satisfacción del Usuario | |

---

# SLI / SLO / SLA

## Service Level Indicators

Documentar.

---

## Service Level Objectives

Documentar.

---

## Service Level Agreements

Documentar.

---

# Dashboards

Documentar los paneles requeridos.

Ejemplo.

- Ejecutivo
- Operaciones
- Desarrollo
- Seguridad
- Infraestructura

---

# Alertas

Definir.

| Alerta | Severidad | Acción |
|---------|-----------|--------|
| Error Rate | Alta | |

Documentar:

- umbrales;
- escalamiento;
- responsables.

---

# Gestión de Incidentes

Documentar.

- detección;
- clasificación;
- respuesta;
- recuperación;
- postmortem.

---

# Observabilidad del Negocio

Definir métricas de negocio.

Ejemplo.

- pedidos por minuto;
- pagos exitosos;
- consentimientos registrados;
- pacientes atendidos.

---

# Observabilidad Técnica

Documentar.

- CPU;
- memoria;
- disco;
- red;
- conexiones;
- errores.

---

# Observabilidad de Seguridad

Documentar.

- autenticaciones;
- intentos fallidos;
- accesos privilegiados;
- anomalías.

---

# Observabilidad de IA

Cuando aplique.

Documentar.

- tokens;
- latencia;
- alucinaciones;
- precisión;
- costo.

---

# Herramientas

Documentar.

- OpenTelemetry
- Prometheus
- Grafana
- Azure Monitor
- CloudWatch
- New Relic
- Dynatrace
- Elastic
- Splunk

Justificar la selección.

---

# Automatización

Documentar.

- Auto Healing
- Escalamiento Automático
- Runbooks
- Workflows
- Respuesta automática

---

# Riesgos

| Riesgo | Mitigación |
|---------|------------|
| Observabilidad insuficiente | |
| Exceso de alertas | |
| Datos incompletos | |
| Costos elevados | |

---

# ADR Relacionados

Referenciar decisiones.

---

# Checklist

## Instrumentación

- [ ] Logs estructurados
- [ ] Métricas definidas
- [ ] Trazabilidad distribuida

---

## Operación

- [ ] Dashboards
- [ ] Alertas
- [ ] Runbooks

---

## Negocio

- [ ] KPIs definidos
- [ ] Métricas de negocio
- [ ] SLO definidos

---

## Gobernanza

- [ ] ADR registrados
- [ ] Responsables definidos
- [ ] Postmortem documentado

---

# Documentos Relacionados

- Enterprise Architecture
- Solution Architecture
- Software Architecture
- Deployment Architecture
- Security Architecture
- SRE Playbook
- Incident Response Playbook
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
| SRE Lead | | |
| Arquitecto | | |
| Operaciones | | |

---

# Declaración Final

La Arquitectura de Observabilidad define cómo una organización obtiene evidencia confiable sobre el comportamiento de sus sistemas para reducir la incertidumbre operacional y acelerar la toma de decisiones.

Su objetivo no es únicamente recopilar datos, sino transformarlos en información útil que permita detectar, comprender, resolver y prevenir incidentes, fortaleciendo la resiliencia y la mejora continua.

---

> **Monitorear es saber que algo falló.**

> **Observar es comprender por qué ocurrió y cómo evitar que vuelva a suceder.**

> **La observabilidad convierte datos en conocimiento operativo.**

---

© Arquetipo Digital
