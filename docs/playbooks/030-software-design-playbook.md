---
title: Playbook de Diseño de Software
id: PB-030
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
  - ARC-SW-110 Software Architecture
  - ARC-QA-210 Quality Attributes
  - ARC-GOV-200 Governance Architecture
  - ADS-004 Architecture Decision Standard
tags:
  - software
  - architecture
  - playbook
---

# Playbook de Diseño de Software

> Un buen software no comienza escribiendo código.
>
> Comienza definiendo claramente las responsabilidades del dominio.

---

# Propósito

Este playbook define el proceso oficial para diseñar software dentro del framework ARCHE.

Su objetivo es asegurar que las soluciones sean:

- comprensibles;
- mantenibles;
- desacopladas;
- escalables;
- preparadas para evolucionar.

---

# Principios

Todo diseño debe respetar los principios de ARCHE.

- El dominio dirige el diseño.
- El software expresa capacidades del negocio.
- Las dependencias apuntan hacia el dominio.
- El desacoplamiento tiene prioridad sobre la reutilización prematura.
- La simplicidad es una decisión arquitectónica.

---

# Flujo General

```text
Problema

↓

Dominio

↓

Responsabilidades

↓

Límites

↓

Componentes

↓

Contratos

↓

Patrones

↓

Dependencias

↓

Implementación
```

---

# Paso 1. Comprender el Dominio

Responder.

- ¿Qué problema resuelve el sistema?
- ¿Qué lenguaje utiliza el negocio?
- ¿Qué reglas son críticas?

No comenzar por la base de datos.

No comenzar por la API.

---

# Paso 2. Identificar Responsabilidades

Separar responsabilidades.

Ejemplo.

- Usuarios
- Consentimientos
- Pagos
- Catálogo
- Notificaciones

Cada responsabilidad debe tener un propósito claro.

---

# Paso 3. Definir Límites

Identificar límites naturales.

Ejemplos.

- Bounded Contexts
- Módulos
- Componentes

Evitar componentes gigantes.

---

# Paso 4. Modelar el Dominio

Identificar.

- Entidades
- Objetos de Valor
- Agregados
- Servicios de Dominio
- Eventos de Dominio
- Repositorios

Documentar únicamente aquello que aporte valor.

---

# Paso 5. Definir Componentes

Cada componente debe responder.

- ¿Qué hace?
- ¿Qué no hace?
- ¿Qué expone?
- ¿Qué consume?

---

# Paso 6. Diseñar Contratos

Todo intercambio entre componentes debe realizarse mediante contratos explícitos.

Ejemplos.

- Interfaces
- APIs
- Eventos
- Comandos
- Consultas

Nunca depender de implementaciones concretas.

---

# Paso 7. Seleccionar Patrones

Elegir únicamente los patrones necesarios.

Ejemplos.

- Clean Architecture
- Arquitectura Hexagonal
- CQRS
- Mediator
- Repository
- Factory
- Strategy
- Decorator
- Adapter

Cada patrón debe justificarse mediante un ADR.

---

# Paso 8. Gestionar Dependencias

Las dependencias deben cumplir.

- Alta cohesión.
- Bajo acoplamiento.
- Inversión de dependencias.
- Separación de responsabilidades.

Verificar la dirección de las dependencias.

---

# Paso 9. Atributos de Calidad

Evaluar.

- mantenibilidad;
- testabilidad;
- escalabilidad;
- resiliencia;
- seguridad;
- observabilidad.

Relacionar con ARC-QA-210.

---

# Paso 10. Diseñar la Persistencia

Responder.

- ¿Qué información pertenece al dominio?
- ¿Qué información es infraestructura?

Evitar que el dominio dependa del ORM.

---

# Paso 11. Diseñar Integraciones

Identificar.

- APIs
- Eventos
- Mensajería
- Batch

Definir contratos antes de implementar.

---

# Paso 12. Diseñar Observabilidad

Todo componente debe producir evidencia.

Documentar.

- logs;
- métricas;
- trazas;
- eventos.

---

# Paso 13. Revisar el Diseño

Realizar una revisión arquitectónica considerando.

- simplicidad;
- claridad;
- cohesión;
- acoplamiento;
- mantenibilidad;
- seguridad.

---

# Artefactos Esperados

| Artefacto | Obligatorio |
|-----------|-------------|
| Software Architecture | ✓ |
| C4 Nivel 3 | ✓ |
| Modelo de Dominio | ✓ |
| ADR | ✓ |
| Diagramas de Componentes | ✓ |

---

# Checklist

## Dominio

- [ ] Lenguaje ubicuo definido.
- [ ] Responsabilidades claras.
- [ ] Límites identificados.

---

## Diseño

- [ ] Componentes definidos.
- [ ] Contratos documentados.
- [ ] Patrones justificados.

---

## Calidad

- [ ] Atributos priorizados.
- [ ] Observabilidad considerada.
- [ ] Seguridad integrada.

---

## Gobernanza

- [ ] ADR registrados.
- [ ] Revisión arquitectónica realizada.
- [ ] Estándares cumplidos.

---

# Antipatrones

Evitar.

- God Object.
- Shared Database sin justificación.
- Acoplamiento circular.
- Clases con múltiples responsabilidades.
- Dependencias hacia infraestructura desde el dominio.
- Lógica de negocio en controladores o capas de presentación.
- Reutilización prematura.
- Abstracciones innecesarias.

---

# Indicadores

| Indicador | Objetivo |
|-----------|----------|
| Cohesión de módulos | Alta |
| Acoplamiento | Bajo |
| Cobertura de pruebas | |
| Complejidad ciclomática | |
| Deuda técnica | |
| ADR implementados | |

---

# Roles

| Rol | Responsabilidad |
|------|-----------------|
| Software Architect | Diseño del software |
| Technical Lead | Implementación técnica |
| Solution Architect | Alineación con la solución |
| QA | Validación técnica |
| Architecture Board | Revisión de decisiones relevantes |

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
Modelo de Dominio
        │
        ▼
Componentes
        │
        ▼
Contratos
        │
        ▼
ADR
        │
        ▼
Implementación
        │
        ▼
Observabilidad
```

---

# Criterios de Éxito

El diseño de software cumple con ARCHE cuando:

- El dominio es el centro de la solución.
- Las responsabilidades están claramente delimitadas.
- Los componentes presentan alta cohesión y bajo acoplamiento.
- Las dependencias respetan la dirección arquitectónica.
- Los patrones utilizados están justificados.
- Las decisiones relevantes se encuentran registradas mediante ADR.
- El software puede evolucionar sin comprometer su coherencia.

---

# Declaración Final

El diseño de software en ARCHE transforma las capacidades del negocio en una estructura técnica coherente, mantenible y preparada para evolucionar.

Su propósito no es producir diagramas o clases, sino construir un modelo de software que exprese claramente el dominio, facilite la comprensión del sistema y reduzca el costo del cambio a lo largo del tiempo.

---

> **El código es una implementación temporal.**
>
> **El diseño de software es la representación duradera del conocimiento del dominio.**
>
> **La mejor arquitectura no es la más compleja, sino la que permite cambiar con confianza.**

---

© Arquetipo Digital
