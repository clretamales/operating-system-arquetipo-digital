---
title: Taxonomía Documental ARCHE
id: MTH-001
version: 1.0
status: Official
owner: Arquetipo Digital
category: Methodology
domain: Documentation
framework: ARCHE
authors:
  - Arquetipo Digital
created: YYYY-MM-DD
last_updated: YYYY-MM-DD
references:
  - DOC-000 Documentation Standard
  - Template System
---

# Taxonomía Documental ARCHE

> Una organización madura no solo produce documentación.
>
> Produce el documento correcto para cada necesidad.

---

# Propósito

La Taxonomía Documental ARCHE define los tipos oficiales de documentos utilizados dentro de Arquetipo Digital.

Su objetivo es establecer un lenguaje común para organizar el conocimiento, evitar duplicidades y facilitar la creación, mantenimiento y evolución de la documentación.

Cada documento cumple un propósito específico dentro de la metodología.

No existen documentos genéricos.

Existen artefactos con objetivos claramente definidos.

---

# Filosofía

No todos los problemas se resuelven con el mismo tipo de documento.

Un estándar no reemplaza una guía.

Un tutorial no reemplaza un playbook.

Un ADR no reemplaza un RFC.

Elegir correctamente el tipo documental reduce complejidad y mejora la comunicación.

---

# Principios

La taxonomía se basa en cinco principios.

## Especialización

Cada documento tiene un único propósito.

---

## Claridad

El lector debe identificar inmediatamente el tipo de documento.

---

## Reutilización

La información debe existir una sola vez.

---

## Trazabilidad

Los documentos deben relacionarse entre sí.

---

## Evolución

La taxonomía puede crecer sin perder coherencia.

---

# Clasificación Oficial

## Foundation

### Propósito

Define la identidad de Arquetipo Digital.

### Responde

> ¿Por qué existimos?

Ejemplos

- Manifiesto
- Principios
- Leyes
- Framework

---

## Methodology

### Propósito

Describe cómo trabajamos.

### Responde

> ¿Cómo hacemos arquitectura?

Ejemplos

- ARCHE
- Discovery Method
- Decision Method

---

## Standard

### Propósito

Define reglas obligatorias.

### Responde

> ¿Qué debe cumplirse?

Ejemplos

- Architecture Standard
- Documentation Standard
- Security Standard

---

## Playbook

### Propósito

Describe procesos repetibles.

### Responde

> ¿Cómo ejecutamos una actividad?

Ejemplos

- Discovery
- Architecture Review
- Modernization

---

## Guide

### Propósito

Comparte experiencia.

### Responde

> ¿Cómo hacerlo correctamente?

Ejemplos

- Guía C4
- Guía ADR
- Guía de Integración

---

## Tutorial

### Propósito

Enseña mediante práctica.

### Responde

> ¿Cómo aprender haciéndolo?

Ejemplos

- Crear un ADR
- Construir un Web Component
- Diseñar un Context Diagram

---

## Reference

### Propósito

Centraliza información de consulta.

### Responde

> ¿Dónde encuentro la información?

Ejemplos

- Glosario
- Convenciones
- APIs
- Catálogo de atributos

---

## ADR

### Propósito

Registrar decisiones arquitectónicas.

### Responde

> ¿Por qué se tomó esta decisión?

---

## RFC

### Propósito

Proponer cambios.

### Responde

> ¿Qué queremos cambiar?

---

## Knowledge

### Propósito

Preservar aprendizaje.

### Responde

> ¿Qué aprendimos?

Ejemplos

- Lecciones Aprendidas
- Casos de Estudio
- Patrones
- Antipatrones

---

# Relación entre documentos

```
Foundation

↓

Methodology

↓

Standards

↓

Templates

↓

Playbooks

↓

Projects

↓

Knowledge
```

Cada tipo documental cumple un rol dentro del ciclo de vida del conocimiento.

---

# Árbol Documental

```
Conocimiento

├── Foundation
│
├── Methodology
│
├── Standards
│
├── Templates
│
├── Playbooks
│
├── Guides
│
├── Tutorials
│
├── References
│
├── ADR
│
├── RFC
│
└── Knowledge
```

La estructura debe mantenerse simple y extensible.

---

# Cómo elegir el documento correcto

| Si necesitas... | Utiliza... |
|-----------------|------------|
| Definir una regla | Standard |
| Explicar un proceso | Playbook |
| Enseñar una buena práctica | Guide |
| Enseñar paso a paso | Tutorial |
| Registrar una decisión | ADR |
| Proponer un cambio | RFC |
| Consultar información | Reference |
| Compartir experiencia | Knowledge |

---

# Ciclo de vida

```
Idea

↓

Método

↓

Estándar

↓

Plantilla

↓

Proyecto

↓

Experiencia

↓

Conocimiento
```

El conocimiento generado vuelve a enriquecer la metodología.

---

# Buenas prácticas

✔ Elegir el tipo documental antes de escribir.

✔ Mantener un único propósito por documento.

✔ Evitar mezclar reglas con tutoriales.

✔ Referenciar documentos relacionados.

✔ Mantener la trazabilidad.

---

# Antipatrones

Evitar:

- documentos híbridos;
- duplicidad de información;
- tutoriales convertidos en estándares;
- playbooks utilizados como documentación técnica;
- conocimiento únicamente verbal.

---

# Declaración Final

La Taxonomía Documental ARCHE representa el lenguaje documental oficial de Arquetipo Digital.

Su propósito es asegurar que el conocimiento se capture, organice y reutilice de forma consistente, permitiendo que la metodología evolucione sin perder claridad ni coherencia.

---

> **Cada documento tiene un propósito.**
>
> **Cada propósito tiene un documento.**

---

© Arquetipo Digital
