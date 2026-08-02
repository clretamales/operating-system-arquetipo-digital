---
title: Playbook de Architecture Decision Records (ADR)
id: PB-010
version: 1.0
status: Official
owner: Arquetipo Digital
category: Playbook
domain: Architecture
framework: ARCHE
authors:
  - Arquetipo Digital
created: 2026-08-02
last_updated: 2026-08-02
next_review: 2027-08-02
references:
  - ADS-004 Architecture Decision Standard
  - ADS-005 Architecture Governance Standard
  - Architecture Review Standard
  - Architecture Quality Attributes
  - Technology Radar
tags:
  - playbook
  - adr
  - architecture
---

# Playbook de Architecture Decision Records (ADR)

> Una decisión no existe hasta que puede ser comprendida, trazada y revisada.

---

# Propósito

Este playbook define el proceso oficial para crear, revisar, aprobar, mantener y retirar un **Architecture Decision Record (ADR)** dentro de la metodología ARCHE.

Su objetivo es asegurar que todas las decisiones arquitectónicas relevantes sean:

- explícitas;
- trazables;
- justificadas;
- revisables;
- gobernadas.

---

# ¿Qué es un ADR?

Un ADR es el registro formal de una decisión arquitectónica que tiene impacto significativo sobre la solución, la organización o la plataforma tecnológica.

No documenta únicamente la decisión.

Documenta también:

- el problema;
- el contexto;
- las alternativas;
- los compromisos (trade-offs);
- las consecuencias;
- la estrategia de revisión.

---

# ¿Cuándo crear un ADR?

Debe crearse un ADR cuando exista alguna de las siguientes situaciones:

- incorporación de una nueva tecnología;
- cambio de patrón arquitectónico;
- modificación de una integración crítica;
- adopción de una plataforma;
- decisión con impacto transversal;
- cambio de estrategia de seguridad;
- decisión que afecte atributos de calidad;
- excepción a un estándar;
- decisión difícil de revertir.

---

# ¿Cuándo NO crear un ADR?

No crear ADR para:

- cambios menores de código;
- refactorizaciones locales;
- configuraciones operativas sin impacto arquitectónico;
- correcciones de errores;
- decisiones temporales sin impacto.

---

# Ciclo de Vida del ADR

```text
Necesidad

↓

Análisis

↓

Alternativas

↓

Evaluación

↓

ADR

↓

Architecture Review

↓

Aprobación

↓

Implementación

↓

Seguimiento

↓

Revisión

↓

Reemplazo o Retiro
```

Un ADR permanece vigente mientras su decisión siga siendo válida.

---

# Flujo del Proceso

## Paso 1. Identificar el problema

Responder:

- ¿Qué decisión debemos tomar?
- ¿Por qué ahora?
- ¿Qué ocurre si no decidimos?

---

## Paso 2. Analizar el contexto

Documentar:

- restricciones;
- dependencias;
- riesgos;
- objetivos;
- stakeholders.

---

## Paso 3. Identificar alternativas

Nunca documentar una única alternativa.

Para cada opción registrar:

- ventajas;
- desventajas;
- riesgos;
- impacto.

---

## Paso 4. Evaluar Trade-Offs

Responder:

- ¿Qué atributo mejora?
- ¿Qué atributo empeora?
- ¿Qué costo introduce?
- ¿Qué complejidad agrega?

Relacionar con:

- Arquitectura de Calidad
- Escenarios de Calidad

---

## Paso 5. Registrar el ADR

Utilizar la plantilla oficial.

El ADR debe incluir:

- contexto;
- decisión;
- alternativas;
- consecuencias;
- revisión futura.

---

## Paso 6. Architecture Review

El ADR debe revisarse considerando:

- alineación con principios;
- cumplimiento de estándares;
- riesgos;
- sostenibilidad;
- impacto organizacional.

---

## Paso 7. Aprobar

El nivel de aprobación dependerá del impacto.

| Impacto | Responsable |
|----------|-------------|
| Bajo | Technical Lead |
| Medio | Solution Architect |
| Alto | Architecture Board |
| Estratégico | Enterprise Architect |

---

## Paso 8. Implementar

Toda implementación debe referenciar el ADR correspondiente.

Ejemplo.

```text
ADR-015
```

en:

- Pull Requests;
- documentación;
- Solution Architecture;
- Software Architecture.

---

## Paso 9. Seguimiento

Durante la operación evaluar:

- ¿La decisión produjo el resultado esperado?
- ¿Aparecieron efectos secundarios?
- ¿Los atributos de calidad mejoraron?

---

## Paso 10. Revisar

Todo ADR debe revisarse periódicamente.

Ejemplo.

- anual;
- cambio tecnológico;
- incidente grave;
- nueva estrategia.

---

## Paso 11. Reemplazar

Cuando una decisión deja de ser válida.

Nunca eliminar un ADR.

Debe quedar:

```text
Superseded by ADR-025
```

---

# Estados Oficiales

| Estado | Descripción |
|----------|-------------|
| Proposed | En elaboración |
| Accepted | Aprobado |
| Implemented | Materializado |
| Deprecated | Próximo al retiro |
| Superseded | Reemplazado |
| Rejected | No aprobado |
| Archived | Histórico |

---

# Criterios de Calidad

Un ADR debe cumplir:

- contexto claro;
- problema explícito;
- alternativas documentadas;
- trade-offs identificados;
- riesgos registrados;
- consecuencias descritas;
- responsable definido.

---

# Matriz de Impacto

Relacionar el ADR con:

| Artefacto | Obligatorio |
|------------|-------------|
| Enterprise Architecture | ✓ |
| Solution Architecture | ✓ |
| Software Architecture | ✓ |
| Quality Attributes | ✓ |
| Technology Radar | ✓ |
| ADR relacionados | ✓ |

---

# Checklist

## Antes de aprobar

- [ ] Problema definido.
- [ ] Contexto documentado.
- [ ] Alternativas evaluadas.
- [ ] Trade-offs registrados.
- [ ] Riesgos identificados.
- [ ] Revisión realizada.

---

## Antes de implementar

- [ ] ADR aprobado.
- [ ] Arquitectura actualizada.
- [ ] Documentación relacionada actualizada.

---

## Durante la operación

- [ ] Indicadores monitoreados.
- [ ] Riesgos revisados.
- [ ] Métricas disponibles.

---

# Antipatrones

Evitar:

- crear ADR después de implementar;
- registrar únicamente la decisión;
- no documentar alternativas;
- eliminar ADR antiguos;
- crear ADR para cambios menores;
- mantener ADR sin revisión.

---

# Indicadores

| Indicador | Objetivo |
|------------|-----------|
| ADR creados | |
| ADR vigentes | |
| ADR revisados | |
| ADR reemplazados | |
| Tiempo de aprobación | |
| ADR sin responsable | |

---

# Relación con ARCHE

```text
Discovery
      │
      ▼
Solution Architecture
      │
      ▼
Software Architecture
      │
      ▼
ADR
      │
      ▼
Architecture Review
      │
      ▼
Implementación
      │
      ▼
Observabilidad
      │
      ▼
Lecciones Aprendidas
      │
      ▼
Nuevo ADR
```

El conocimiento obtenido durante la operación puede originar nuevos ADR.

---

# Roles

| Rol | Responsabilidad |
|------|-----------------|
| Enterprise Architect | Decisiones estratégicas |
| Solution Architect | Decisiones de solución |
| Software Architect | Decisiones técnicas |
| Technical Lead | Implementación |
| Architecture Board | Aprobación |
| Product Owner | Validación del valor de negocio |

---

# Declaración Final

Los Architecture Decision Records constituyen la memoria arquitectónica de la organización.

Cada ADR representa una decisión consciente, respaldada por evidencia, alineada con los principios de ARCHE y preparada para evolucionar a medida que cambian las necesidades del negocio y la tecnología.

Una arquitectura madura no se caracteriza por tener pocas decisiones.

Se caracteriza por comprenderlas, justificarlas y revisarlas de forma sistemática.

---

> **El código explica cómo funciona el sistema.**

> **Los ADR explican por qué el sistema llegó a ser así.**

> **Una organización sin ADR pierde su memoria arquitectónica.**

---

© Arquetipo Digital
