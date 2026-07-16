---
title: Architectural Principles Catalog
version: 1.0
status: Living Document
owner: Arquetipo Digital
last_updated: 2026-07-16
category: Foundation
references:
  - TOGAF
  - ISO/IEC 25010
  - Domain-Driven Design
  - Clean Architecture
---

# Architectural Principles Catalog

> La arquitectura no se construye mediante reglas.
>
> Se construye mediante principios.

---

# Propósito

Este documento define el conjunto oficial de principios arquitectónicos de Arquetipo Digital.

Los principios representan la forma en que analizamos, diseñamos y evolucionamos soluciones.

No son patrones.

No son metodologías.

No son tecnologías.

Son criterios permanentes que orientan toda decisión.

Mientras las herramientas cambian, los principios permanecen.

---

# Clasificación

Nuestros principios se organizan en cuatro dominios.

```text
Pensamiento

Arquitectura

Ingeniería

Evolución
```

Cada nuevo principio deberá pertenecer a uno de estos dominios.

---

# AP-001

# El contexto precede a la tecnología

## Declaración

Nunca elegimos una tecnología antes de comprender el contexto.

---

## Fundamento

Toda tecnología resuelve determinados problemas.

Elegir una herramienta sin comprender el problema conduce a soluciones innecesariamente complejas.

---

## Implicancias

- primero comprender
- después diseñar
- finalmente implementar

---

## Antipatrones

- adoptar tecnologías por moda
- copiar arquitecturas
- sobreingeniería

---

## Relación

TOGAF

DDD

Lean Thinking

---

## Ejemplo

Incorrecto

"Utilizaremos Kubernetes porque es el estándar."

Correcto

"Analizaremos primero si el contexto realmente requiere orquestación."

---

Estado

Official

---

# AP-002

# La arquitectura protege el negocio

## Declaración

Toda decisión arquitectónica debe generar valor para el negocio.

---

## Fundamento

La arquitectura existe para reducir riesgos, facilitar la evolución y proteger la inversión.

No existe para demostrar conocimiento técnico.

---

## Implicancias

Cada decisión debe responder:

¿Qué problema del negocio estamos resolviendo?

---

## Antipatrones

Arquitectura por prestigio.

Complejidad innecesaria.

---

## Relación

TOGAF

Architecture Governance

---

Estado

Official

---

# AP-003

# Diseñar para el cambio

## Declaración

Toda solución debe aceptar el cambio como una condición permanente.

---

## Fundamento

El cambio es inevitable.

La arquitectura debe reducir el costo del cambio.

---

## Implicancias

- desacoplamiento
- modularidad
- interfaces claras
- contratos estables

---

## Antipatrones

Sistemas monolíticos rígidos.

Dependencias circulares.

Acoplamiento excesivo.

---

## Relación

Clean Architecture

SOLID

DDD

---

Estado

Official

---

# AP-004

# La simplicidad es una decisión arquitectónica

## Declaración

La simplicidad no ocurre por accidente.

Debe diseñarse.

---

## Fundamento

La complejidad aumenta naturalmente.

La simplicidad requiere disciplina.

---

## Implicancias

Eliminar lo innecesario.

Reducir capas.

Reducir dependencias.

Reducir reglas.

---

## Antipatrones

Sobreingeniería.

Frameworks innecesarios.

Abstracciones prematuras.

---

## Relación

KISS

YAGNI

Lean

---

Estado

Official

---

# AP-005

# Documentar es construir

## Declaración

La documentación forma parte del producto.

---

## Fundamento

La arquitectura debe sobrevivir a las personas.

---

## Implicancias

Toda decisión importante debe quedar registrada.

---

## Antipatrones

Conocimiento tribal.

Documentación obsoleta.

Arquitectura implícita.

---

## Relación

ADR

Arc42

C4

---

Estado

Official

---

# AP-006

# Los límites crean autonomía

## Declaración

Los sistemas evolucionan mejor cuando sus límites están claramente definidos.

---

## Fundamento

Los límites reducen el acoplamiento.

Facilitan la evolución.

Permiten escalar equipos.

---

## Implicancias

- bounded contexts
- APIs
- contratos
- ownership

---

## Antipatrones

Bases de datos compartidas.

Dependencias ocultas.

Integraciones directas.

---

## Relación

DDD

Team Topologies

Microservices

---

Estado

Official

---

# AP-007

# La calidad es responsabilidad de la arquitectura

## Declaración

La calidad no se inspecciona.

Se diseña.

---

## Fundamento

Los atributos de calidad deben estar presentes desde la primera decisión.

---

## Implicancias

Toda arquitectura deberá proteger:

- seguridad
- rendimiento
- observabilidad
- resiliencia
- mantenibilidad

---

## Antipatrones

Agregar calidad al final del proyecto.

---

## Relación

ISO 25010

Software Architecture in Practice

---

Estado

Official

---

# AP-008

# Toda decisión debe poder justificarse

## Declaración

Las decisiones arquitectónicas deben ser transparentes.

---

## Fundamento

Las mejores decisiones pueden explicarse.

Las peores suelen depender únicamente de opiniones.

---

## Implicancias

Toda decisión relevante requiere:

- contexto
- alternativas
- consecuencias

---

## Antipatrones

"Siempre lo hemos hecho así."

---

## Relación

ADR

Architecture Reviews

---

Estado

Official

---

# Ciclo de Vida

Cada principio puede tener uno de los siguientes estados.

| Estado | Descripción |
|----------|-------------|
| Draft | En discusión. |
| Proposed | Pendiente de validación. |
| Official | Adoptado oficialmente. |
| Deprecated | No se recomienda para nuevos proyectos. |
| Archived | Conservado únicamente por razones históricas. |

---

# Gobernanza

Los principios son patrimonio intelectual de Arquetipo Digital.

Su modificación requiere:

- revisión arquitectónica;
- justificación técnica;
- evaluación de impacto;
- actualización de la documentación relacionada.

---

# Regla Fundamental

Las metodologías evolucionan.

Los frameworks aparecen y desaparecen.

Las plataformas cambian.

Los principios permanecen.

---

> Una arquitectura sólida no se reconoce por la cantidad de tecnologías que utiliza.

> Se reconoce porque sus principios siguen siendo válidos muchos años después de haber sido construida.
