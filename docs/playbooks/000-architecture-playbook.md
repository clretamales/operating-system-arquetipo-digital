---
title: Architecture Playbook
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-20
category: Playbook
framework: ARCHE
---

# Architecture Playbook

> "La arquitectura no es un entregable.
>
> Es una disciplina."

---

# Propósito

Este Playbook define la metodología operativa utilizada por Arquetipo Digital para abordar cualquier iniciativa de arquitectura, desarrollo o transformación digital.

Su propósito es garantizar que todos los proyectos compartan una misma forma de pensar, diseñar, documentar y evolucionar.

No importa si el proyecto consiste en:

- una Landing Page
- una API
- una Plataforma SaaS
- una Arquitectura Empresarial
- una Modernización
- una Integración
- una solución basada en IA

El proceso siempre comienza de la misma manera.

---

# Filosofía

No comenzamos escribiendo código.

No comenzamos diseñando interfaces.

No comenzamos eligiendo tecnologías.

Comenzamos comprendiendo.

Todo proyecto es primero un problema.

Luego un sistema.

Finalmente una implementación.

---

# Nuestro Modelo Operacional

Todo proyecto recorre cinco etapas.

```text
          ARCHE

 Analyze

      ↓

 Reason

      ↓

 Create

      ↓

 Harmonize

      ↓

 Evolve
```

Cada etapa produce conocimiento.

Cada etapa reduce incertidumbre.

Cada etapa tiene entregables.

---

# Etapa 1

# Analyze

## Objetivo

Comprender completamente el problema.

Nunca diseñamos soluciones para requisitos.

Diseñamos soluciones para necesidades.

---

## Preguntas

¿Por qué existe este proyecto?

¿Qué problema resuelve?

¿Quién recibe valor?

¿Qué riesgos existen?

¿Qué restricciones existen?

¿Qué procesos participan?

¿Qué duele hoy?

---

## Actividades

✔ Workshops

✔ Discovery

✔ Entrevistas

✔ Levantamiento

✔ Context Mapping

✔ Stakeholders

✔ Event Storming (si aplica)

---

## Artefactos

- Problem Statement
- Context Diagram
- Stakeholders
- Context Map
- Objetivos del negocio
- Restricciones

---

## Criterio de salida

Todos los participantes comprenden el mismo problema.

---

# Etapa 2

# Reason

## Objetivo

Transformar información en decisiones.

---

## Actividades

- evaluar alternativas
- identificar riesgos
- analizar impacto
- analizar costo del cambio
- atributos de calidad
- trade-offs

---

## Herramientas

- Decision Matrix

- Quality Attributes

- Architectural Decision Model

- ADR Draft

---

## Artefactos

- Matriz de alternativas

- Riesgos

- Restricciones

- Decisiones candidatas

---

## Criterio de salida

Existe una alternativa claramente justificada.

---

# Etapa 3

# Create

## Objetivo

Diseñar la arquitectura.

---

## Actividades

Diseño de:

- Arquitectura Empresarial

- Arquitectura de Solución

- Arquitectura de Software

- UX

- APIs

- Datos

- Seguridad

- Cloud

---

## Diagramas

Preferimos:

- C4

- Sequence

- BPMN

- Domain Model

- Event Flow

---

## Artefactos

- Arquitectura

- Diagramas

- ADR

- Modelos

- Componentes

---

## Criterio de salida

La solución puede ser comprendida antes de implementarse.

---

# Etapa 4

# Harmonize

## Objetivo

Validar coherencia.

---

## Validamos

Negocio

↓

Arquitectura

↓

UX

↓

Operación

↓

Seguridad

↓

Infraestructura

↓

Desarrollo

---

## Revisiones

Architecture Review

Security Review

UX Review

Business Review

Operational Review

---

## Resultado

Arquitectura aprobada.

---

# Etapa 5

# Evolve

## Objetivo

Aprender continuamente.

---

## Actividades

Implementación

↓

Observabilidad

↓

Feedback

↓

Métricas

↓

ADR nuevos

↓

Refinamiento

↓

Roadmap

---

## Artefactos

Lessons Learned

Architecture Score

Roadmap

Nuevos Principios

Nuevos ADR

---

## Criterio de salida

La arquitectura mejora continuamente.

---

# Checkpoints

Antes de avanzar de etapa verificamos.

## Analyze

□ Problema comprendido

□ Stakeholders identificados

□ Restricciones conocidas

---

## Reason

□ Alternativas evaluadas

□ Trade-offs documentados

□ Riesgos conocidos

---

## Create

□ Diagramas completos

□ Arquitectura documentada

□ Calidad evaluada

---

## Harmonize

□ Revisiones realizadas

□ ADR aprobados

□ Riesgos aceptados

---

## Evolve

□ Métricas disponibles

□ Roadmap actualizado

□ Lecciones aprendidas registradas

---

# Documentos obligatorios

Todo proyecto deberá generar como mínimo.

```text
Problem Statement

↓

Architecture Overview

↓

Architecture Decision Records

↓

Quality Attribute Analysis

↓

Solution Architecture

↓

Deployment Architecture

↓

Lessons Learned
```

---

# Definition of Ready (DoR)

Una iniciativa está lista para comenzar cuando:

- el problema está definido;
- existe patrocinio;
- los objetivos son claros;
- se conocen las restricciones;
- existe un contexto compartido.

---

# Definition of Done (DoD)

Una arquitectura está terminada cuando:

- puede implementarse;
- puede evolucionar;
- está documentada;
- protege los atributos de calidad;
- posee ADR;
- puede explicarse sin depender de su autor.

---

# Roles

## Arquitecto

Diseña.

Conecta.

Cuestiona.

Protege la arquitectura.

---

## Consultor

Comprende el negocio.

Facilita decisiones.

Reduce incertidumbre.

---

## Desarrollador

Implementa la arquitectura.

Retroalimenta el diseño.

Documenta aprendizaje.

---

## Cliente

Define objetivos.

Valida valor.

Aporta contexto.

---

# Principios Operacionales

Todo proyecto debe:

✔ Comprender antes de construir.

✔ Diseñar antes de implementar.

✔ Documentar antes de olvidar.

✔ Validar antes de escalar.

✔ Evolucionar continuamente.

---

# Nuestro estándar

No entregamos únicamente software.

Entregamos arquitectura.

No entregamos únicamente documentación.

Entregamos conocimiento.

No entregamos únicamente soluciones.

Entregamos capacidades para evolucionar.

---

# Declaración Final

El éxito de un proyecto no se mide por la velocidad con la que se entrega.

Se mide por la facilidad con la que podrá evolucionar dentro de cinco años.

---

> Construimos sistemas que otros puedan comprender.
>
> Diseñamos arquitecturas que otros puedan continuar.
>
> Documentamos conocimiento que otros puedan aprovechar.

---

© Arquetipo Digital
