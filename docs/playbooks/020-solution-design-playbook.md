---
title: Playbook de Diseño de Soluciones
id: PB-020
version: 1.0
status: Official
owner: Arquetipo Digital
category: Playbook
framework: ARCHE
authors:
  - Arquetipo Digital
created: 2026-08-02
last_updated: 2026-08-02
references:
  - MTH-002 Architecture Lifecycle
  - ARC-SOL-100 Solution Architecture
  - ARC-EA-120 Enterprise Architecture
  - ARC-QA-210 Quality Attributes
  - ARC-GOV-200 Governance Architecture
tags:
  - playbook
  - solution
  - architecture
---

# Playbook de Diseño de Soluciones

> Una buena solución no comienza con tecnología.
>
> Comienza comprendiendo el problema que el negocio necesita resolver.

---

# Propósito

Este playbook define el proceso oficial para diseñar una solución utilizando la metodología ARCHE.

Su objetivo es garantizar que toda solución:

- responda a una necesidad real;
- esté alineada con la estrategia;
- sea técnicamente sostenible;
- genere decisiones trazables;
- pueda evolucionar con el tiempo.

---

# Principios

Todo diseño debe seguir los principios de ARCHE.

- Comprender antes de diseñar.
- Diseñar antes de implementar.
- Justificar antes de decidir.
- Simplificar antes de optimizar.
- Evolucionar antes que reemplazar.

---

# Flujo General

```text
Necesidad

↓

Discovery

↓

Contexto

↓

Capacidades

↓

Restricciones

↓

Escenarios

↓

Alternativas

↓

Trade-Offs

↓

Decisiones

↓

Arquitectura

↓

Validación

↓

Roadmap
```

---

# Paso 1. Comprender la Necesidad

## Objetivo

Entender claramente el problema.

Responder:

- ¿Qué necesita el negocio?
- ¿Qué problema existe?
- ¿Cuál es el impacto?
- ¿Cuál es el valor esperado?

---

# Paso 2. Discovery

Realizar:

- entrevistas;
- workshops;
- revisión documental;
- análisis de procesos;
- análisis de sistemas existentes.

---

## Entregables

- Discovery Report
- Stakeholders
- Context Diagram

---

# Paso 3. Contexto

Documentar.

## Alcance

## Restricciones

## Supuestos

## Dependencias

## Riesgos

---

# Paso 4. Capacidades

Identificar.

- capacidades actuales;
- capacidades futuras;
- capacidades críticas.

Relacionar con Enterprise Architecture.

---

# Paso 5. Drivers Arquitectónicos

Documentar.

Ejemplos.

- crecimiento;
- regulación;
- experiencia usuario;
- disponibilidad;
- escalabilidad;
- costos.

Priorizar.

---

# Paso 6. Atributos de Calidad

Seleccionar únicamente los atributos realmente importantes.

Ejemplo.

| Atributo | Prioridad |
|----------|-----------|
| Seguridad | Alta |
| Disponibilidad | Alta |
| Escalabilidad | Media |

Relacionar con ARC-QA-210.

---

# Paso 7. Escenarios

Construir escenarios.

Ejemplo.

- escenario normal;
- crecimiento;
- falla;
- contingencia.

---

# Paso 8. Alternativas

Nunca diseñar una única opción.

Para cada alternativa documentar.

- beneficios;
- riesgos;
- complejidad;
- costo;
- impacto.

---

# Paso 9. Trade-Offs

Responder.

- ¿Qué ganamos?
- ¿Qué perdemos?
- ¿Qué atributos mejoran?
- ¿Qué atributos empeoran?

Relacionar con ADR.

---

# Paso 10. Selección

Seleccionar la alternativa utilizando criterios objetivos.

Ejemplo.

| Criterio | Peso |
|----------|-----:|
| Valor negocio | 30% |
| Calidad | 25% |
| Riesgo | 20% |
| Complejidad | 15% |
| Coste | 10% |

Registrar la justificación.

---

# Paso 11. Arquitectura

Construir.

- Context Diagram
- C4 Nivel 1
- C4 Nivel 2
- C4 Nivel 3
- Integraciones
- Datos
- Seguridad
- Observabilidad

Utilizar el template de Solution Architecture.

---

# Paso 12. ADR

Registrar las decisiones relevantes.

Toda decisión importante debe generar un ADR.

---

# Paso 13. Validación

Realizar Architecture Review.

Evaluar.

- alineación estratégica;
- estándares;
- riesgos;
- sostenibilidad;
- calidad.

---

# Paso 14. Roadmap

Definir.

- Quick Wins
- MVP
- Evolución
- Modernización

---

# Artefactos Esperados

| Artefacto | Obligatorio |
|-----------|-------------|
| Discovery | ✓ |
| Context Diagram | ✓ |
| Capability Map | ✓ |
| Solution Architecture | ✓ |
| ADR | ✓ |
| Roadmap | ✓ |

---

# Checklist

## Discovery

- [ ] Problema comprendido
- [ ] Stakeholders identificados
- [ ] Restricciones documentadas

---

## Diseño

- [ ] Alternativas evaluadas
- [ ] Trade-offs registrados
- [ ] Atributos priorizados

---

## Arquitectura

- [ ] Diagramas creados
- [ ] Integraciones definidas
- [ ] Riesgos documentados

---

## Gobernanza

- [ ] ADR creados
- [ ] Architecture Review realizada
- [ ] Estándares cumplidos

---

# Antipatrones

Evitar:

- comenzar por una tecnología;
- diseñar sin comprender el negocio;
- copiar soluciones anteriores sin evaluación;
- elegir una alternativa sin comparar opciones;
- documentar al finalizar el desarrollo;
- ignorar los atributos de calidad.

---

# Indicadores

| Indicador | Objetivo |
|-----------|----------|
| Tiempo de Discovery | |
| Alternativas evaluadas | |
| ADR creados | |
| Riesgos mitigados | |
| Reutilización de componentes | |

---

# Roles

| Rol | Responsabilidad |
|------|-----------------|
| Sponsor | Priorizar el valor de negocio |
| Product Owner | Definir necesidades |
| Enterprise Architect | Alineación estratégica |
| Solution Architect | Diseño de la solución |
| Technical Lead | Factibilidad técnica |
| Security Architect | Riesgos y controles |
| Architecture Board | Validación final |

---

# Relación con ARCHE

```text
Necesidad
        │
        ▼
Discovery
        │
        ▼
Enterprise Architecture
        │
        ▼
Solution Architecture
        │
        ▼
Quality Attributes
        │
        ▼
ADR
        │
        ▼
Architecture Review
        │
        ▼
Roadmap
        │
        ▼
Implementación
```

---

# Criterios de Éxito

Una solución diseñada con ARCHE debe cumplir los siguientes criterios:

- Está alineada con una necesidad del negocio.
- Justifica sus decisiones mediante ADR.
- Prioriza atributos de calidad.
- Considera riesgos y restricciones.
- Mantiene trazabilidad entre estrategia, diseño e implementación.
- Puede evolucionar sin comprometer la coherencia arquitectónica.

---

# Declaración Final

El diseño de soluciones en ARCHE es un proceso de razonamiento estructurado que transforma una necesidad del negocio en una arquitectura sostenible.

El objetivo no es producir diagramas, sino construir una comprensión compartida que permita tomar decisiones conscientes, reducir la incertidumbre y facilitar la evolución continua de la solución.

---

> **Una solución no se mide por la cantidad de tecnología que incorpora.**
>
> **Se mide por la claridad con que resuelve un problema y por su capacidad de seguir haciéndolo cuando el contexto cambia.**

---

© Arquetipo Digital
