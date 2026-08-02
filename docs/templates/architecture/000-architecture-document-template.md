---
title: <Título del Documento de Arquitectura>
id: ARC-000
version: 1.0
status: Draft
owner: Arquetipo Digital
category: Architecture
domain: <Solution | Software | Enterprise | Cloud | Integration | Data | AI>
framework: ARCHE
classification: <Conceptual | Logical | Physical | Deployment>
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
  - ADS-000 Architecture Document Standard
  - ADS-001 C4 Model Standard
  - ADS-002 Architecture Review Standard
  - ADS-003 Quality Attribute Scenarios
  - ADS-004 Architecture Decision Standard
tags:
  - architecture
---

# <Título del Documento>

> **La arquitectura no describe únicamente una solución.**
>
> **Describe las decisiones que permiten construirla y evolucionarla.**

---

# Resumen Ejecutivo

## Propósito

Describir en una página:

- Problema
- Objetivo
- Solución propuesta
- Beneficios esperados
- Riesgos principales

Este resumen debe ser comprensible por perfiles técnicos y de negocio.

---

# Información General

| Campo | Valor |
|--------|-------|
| Proyecto | |
| Cliente | |
| Dominio | |
| Responsable | |
| Estado | |
| Versión | |

---

# Contexto del Negocio

## Situación actual

Describir el contexto.

Responder:

- ¿Qué ocurre actualmente?
- ¿Qué problema existe?
- ¿Quiénes son los actores?

---

## Necesidad

¿Qué necesidad motiva esta arquitectura?

---

## Objetivos

### Objetivos de Negocio

- Objetivo

### Objetivos Arquitectónicos

- Objetivo

### Objetivos Técnicos

- Objetivo

---

# Alcance

## Incluye

- Alcance

## No incluye

- Exclusiones

## Supuestos

- Supuesto

## Restricciones

- Restricción

---

# Stakeholders

| Rol | Responsabilidad |
|------|-----------------|
| Sponsor | |
| Product Owner | |
| Arquitecto | |
| Equipo | |
| Operaciones | |

---

# Estado Actual (AS-IS)

Describir la arquitectura actual.

Incluir cuando corresponda:

- Context Diagram
- Landscape
- Procesos
- Integraciones
- Sistemas existentes

---

# Problemas Identificados

Documentar los principales problemas.

| Problema | Impacto |
|----------|---------|
| Problema | Impacto |

---

# Atributos de Calidad

Priorizar los atributos de calidad.

| Atributo | Prioridad | Justificación |
|----------|-----------|---------------|
| Seguridad | Alta | |
| Escalabilidad | Media | |
| Observabilidad | Alta | |
| Rendimiento | Alta | |

Referenciar ADS-003 cuando corresponda.

---

# Principios Arquitectónicos Aplicados

Relacionar los principios utilizados.

| Principio | Justificación |
|------------|---------------|
| AP-001 | |
| AP-004 | |

---

# Alternativas Evaluadas

## Alternativa A

### Ventajas

-

### Desventajas

-

### Riesgos

-

---

## Alternativa B

...

---

# Decisión Arquitectónica

Explicar:

- alternativa seleccionada;
- motivos;
- trade-offs;
- beneficios esperados.

Referenciar el ADR correspondiente.

---

# Arquitectura Objetivo (TO-BE)

## Vista de Contexto

Agregar diagrama C4 Nivel 1.

---

## Vista de Contenedores

Agregar diagrama C4 Nivel 2.

---

## Vista de Componentes

Agregar diagrama C4 Nivel 3 cuando aplique.

---

## Vista de Despliegue

Agregar Deployment Diagram cuando corresponda.

---

## Integraciones

Documentar:

- APIs
- Eventos
- Mensajería
- Protocolos

---

## Modelo de Datos

Cuando corresponda incluir:

- entidades;
- dominios;
- agregados;
- relaciones.

---

# Seguridad

Documentar:

- autenticación;
- autorización;
- cifrado;
- auditoría;
- gestión de secretos.

---

# Observabilidad

Documentar:

- logging;
- métricas;
- trazabilidad;
- alertas;
- dashboards.

---

# Operación

Describir:

- monitoreo;
- respaldo;
- recuperación;
- escalamiento;
- continuidad.

---

# Riesgos

| Riesgo | Probabilidad | Impacto | Mitigación |
|----------|--------------|----------|------------|
| Riesgo | | | |

---

# Dependencias

| Dependencia | Tipo | Estado |
|--------------|------|--------|
| Dependencia | | |

---

# Roadmap

```text
Fase 1

↓

Fase 2

↓

Fase 3

↓

Optimización

↓

Evolución Continua
```

---

# Criterios de Aceptación

La arquitectura será considerada aprobada cuando:

- [ ] Cumpla los objetivos del negocio.
- [ ] Cumpla los atributos de calidad.
- [ ] Supere la revisión arquitectónica.
- [ ] Existan ADR para decisiones relevantes.
- [ ] La documentación esté completa.

---

# Checklist Arquitectónico

## Negocio

- [ ] Contexto comprendido.
- [ ] Stakeholders identificados.
- [ ] Objetivos claros.

---

## Arquitectura

- [ ] Alternativas evaluadas.
- [ ] Decisiones justificadas.
- [ ] Diagramas actualizados.

---

## Calidad

- [ ] Escenarios documentados.
- [ ] Riesgos identificados.
- [ ] Observabilidad considerada.

---

## Gobernanza

- [ ] Revisión realizada.
- [ ] ADR registrados.
- [ ] Excepciones documentadas.

---

# Documentos Relacionados

## Foundation

- Framework ARCHE

---

## Standards

- ADS-000
- ADS-001
- ADS-002
- ADS-003
- ADS-004
- ADS-005

---

## Playbooks

- Architecture Playbook

---

## ADR

- ADR-XXX

---

# Historial de Versiones

| Versión | Fecha | Descripción |
|----------|------|-------------|
| 1.0 | YYYY-MM-DD | Primera versión |

---

# Aprobaciones

| Rol | Responsable | Fecha |
|------|-------------|------|
| Autor | | |
| Revisor | | |
| Aprobador | | |

---

# Declaración Final

La arquitectura representa un acuerdo entre el negocio y la tecnología.

Este documento registra el contexto, las decisiones y la visión necesaria para construir una solución sostenible, comprensible y preparada para evolucionar.

---

> **Una buena arquitectura no solo explica cómo construir un sistema.**
>
> **Explica por qué fue construido de esa manera y cómo podrá evolucionar mañana.**

---

© Arquetipo Digital
