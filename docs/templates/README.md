---
title: Template System
id: TMP-000
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-20
category: Templates
domain: Documentation
framework: ARCHE
references:
  - DOC-000 Documentation Standard
  - ADS-000 Architecture Document Standard
  - ADS-004 Architecture Decision Standard
  - ADS-005 Architecture Governance Standard
---

# Template System

> La calidad de una práctica arquitectónica no depende únicamente de sus estándares.
>
> También depende de que cada profesional pueda aplicarlos de manera consistente.

---

# Propósito

El **Template System** proporciona un conjunto de plantillas oficiales para la creación de documentos dentro del ecosistema de Arquetipo Digital.

Su objetivo es acelerar la generación de contenido, reducir la variabilidad entre entregables y garantizar el cumplimiento de los estándares definidos por la organización.

Las plantillas representan la implementación práctica de la metodología ARCHE.

---

# Filosofía

Los estándares responden **qué** debe cumplir un documento.

Las plantillas responden **cómo** comenzar a construirlo.

De esta forma, los consultores pueden concentrarse en el contenido y no en la estructura.

---

# Objetivos

El Template System busca:

- estandarizar la estructura de los documentos;
- reducir el tiempo de elaboración;
- facilitar revisiones;
- mejorar la calidad documental;
- preservar la consistencia entre proyectos;
- favorecer la reutilización del conocimiento.

---

# Organización

Las plantillas se organizan según su propósito.

```text
templates/

architecture/
decisions/
documentation/
governance/
operations/
proposals/
workshops/
ai/
examples/
```

Cada carpeta representa un dominio específico dentro de la práctica de arquitectura.

---

# Arquitectura

Plantillas utilizadas para diseñar soluciones.

Ejemplos:

- Architecture Document
- Solution Architecture
- Enterprise Architecture
- Cloud Architecture
- Integration Architecture
- AI Architecture

---

# Decisiones

Plantillas destinadas al registro y análisis de decisiones arquitectónicas.

Ejemplos:

- ADR
- Decision Record
- Trade-off Analysis
- Exception Request

---

# Documentación

Plantillas para documentación institucional.

Ejemplos:

- Standard
- Guide
- Playbook
- Tutorial
- Knowledge Base
- Glossary

---

# Gobernanza

Plantillas para procesos de revisión y control.

Ejemplos:

- Architecture Review
- Governance Checklist
- Quality Gate
- Architecture Board Minutes

---

# Operaciones

Documentación utilizada durante la ejecución de proyectos.

Ejemplos:

- Meeting Notes
- Lessons Learned
- Retrospective
- Incident Postmortem

---

# Propuestas

Documentos utilizados durante actividades de consultoría.

Ejemplos:

- Consulting Proposal
- Assessment Report
- Executive Summary
- Roadmap

---

# Workshops

Plantillas para sesiones colaborativas.

Ejemplos:

- Discovery Workshop
- Event Storming
- Quality Attribute Workshop
- Architecture Workshop

---

# Inteligencia Artificial

Plantillas diseñadas para colaborar con asistentes de IA.

Ejemplos:

- Architecture Prompt
- ADR Prompt
- Review Prompt
- Documentation Prompt
- Coding Agent Context

Estas plantillas permiten que herramientas de IA generen contenido alineado con los estándares de Arquetipo Digital.

---

# Ejemplos

La carpeta `examples` contiene documentos completos elaborados utilizando las plantillas oficiales.

Su objetivo es mostrar el nivel de calidad esperado y servir como referencia para nuevos consultores.

Una plantilla explica la estructura.

Un ejemplo demuestra el resultado esperado.

---

# Convenciones

Todas las plantillas deben:

- seguir el Documentation Standard;
- incluir metadatos;
- utilizar títulos consistentes;
- incorporar referencias cruzadas cuando corresponda;
- mantener una estructura clara y reutilizable.

Las plantillas no contienen contenido específico de un proyecto.

Solo proporcionan la estructura base.

---

# Uso recomendado

El flujo sugerido para elaborar un documento es:

```text
Seleccionar plantilla

↓

Completar metadatos

↓

Agregar contexto

↓

Desarrollar contenido

↓

Revisar cumplimiento de estándares

↓

Publicar

↓

Mantener
```

---

# Relación con ARCHE

| Etapa | Uso del Template System |
|--------|-------------------------|
| Analyze | Registrar descubrimientos y contexto |
| Reason | Documentar alternativas y decisiones |
| Create | Elaborar diseños y entregables |
| Harmonize | Facilitar revisiones y gobernanza |
| Evolve | Actualizar documentación y preservar aprendizajes |

El sistema de plantillas acompaña todas las fases de la metodología ARCHE.

---

# Buenas prácticas

✔ Seleccionar la plantilla adecuada antes de comenzar.

✔ Mantener la estructura original.

✔ Adaptar únicamente el contenido.

✔ Referenciar estándares relacionados.

✔ Eliminar secciones que no apliquen, en lugar de dejarlas vacías.

✔ Mantener ejemplos separados de las plantillas.

---

# Antipatrones

Evitar:

- crear documentos desde cero cuando existe una plantilla oficial;
- modificar la estructura sin justificación;
- duplicar plantillas con pequeñas variaciones;
- incluir contenido específico de clientes dentro de las plantillas;
- utilizar una plantilla para un propósito distinto al definido.

---

# Evolución del Template System

El Template System es un activo vivo.

Las nuevas plantillas deberán:

- responder a una necesidad recurrente;
- alinearse con los estándares existentes;
- evitar duplicidad con plantillas ya disponibles;
- ser revisadas antes de incorporarse al repositorio oficial.

---

# Declaración Final

Las plantillas representan la materialización práctica de los estándares de Arquetipo Digital.

Su propósito no es limitar la creatividad, sino proporcionar una base consistente sobre la cual los equipos puedan construir soluciones de alta calidad de forma eficiente y repetible.

---

> **Los estándares definen la calidad esperada.**
>
> **Las plantillas permiten alcanzarla de manera consistente.**

---

© Arquetipo Digital — Template System
