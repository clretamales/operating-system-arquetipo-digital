---
title: Architectural Laws
version: 1.0
status: Constitutional
owner: Arquetipo Digital
last_updated: 2026-07-16
category: Foundation
references:
  - Architectural Thinking
  - Architectural Decision Model
  - Architectural Principles Catalog
---

# Architectural Laws

> La arquitectura no solamente necesita principios.
>
> Necesita límites.

---

# Introducción

Las Leyes Arquitectónicas representan los acuerdos fundamentales e inquebrantables de Arquetipo Digital.

Mientras los principios orientan nuestras decisiones, las leyes establecen aquello que nunca estamos dispuestos a comprometer.

Estas leyes constituyen la base de nuestra identidad como firma de arquitectura digital.

Toda excepción deberá justificarse explícitamente mediante una revisión arquitectónica.

---

# Ley 1
## La arquitectura siempre precede a la implementación.

Nunca comenzamos construyendo.

Primero comprendemos.

Después diseñamos.

Finalmente implementamos.

Ninguna solución tecnológica debe existir sin una arquitectura que la sostenga.

### Implicancias

- No desarrollamos sin comprender el negocio.
- No escribimos código sin diseño.
- No elegimos tecnologías sin contexto.

---

# Ley 2
## Ninguna decisión importante puede existir sin documentación.

Toda decisión relevante debe quedar registrada.

La memoria de las personas no constituye documentación.

El conocimiento pertenece a la organización.

Nunca a un individuo.

### Implicancias

Toda decisión deberá generar evidencia mediante:

- ADR
- Diagramas
- Principios
- Documentación técnica

---

# Ley 3
## El contexto determina la solución.

No existen arquitecturas universales.

No existen tecnologías perfectas.

Toda decisión depende del contexto.

Copiar soluciones sin comprender el problema está prohibido.

### Implicancias

Antes de proponer una solución debemos comprender:

- negocio
- usuarios
- restricciones
- capacidades
- riesgos

---

# Ley 4
## La simplicidad es obligatoria.

La complejidad debe justificarse.

Nunca al revés.

Cada componente, dependencia o capa adicional aumenta el costo futuro del sistema.

La arquitectura debe minimizar esa complejidad.

### Implicancias

Siempre preferiremos:

- menos componentes
- menos dependencias
- menos reglas
- menos tecnología

Siempre que el negocio lo permita.

---

# Ley 5
## Todo sistema debe poder evolucionar.

Diseñar para el presente genera deuda.

Diseñar para la evolución genera sostenibilidad.

Ninguna arquitectura debe impedir el cambio.

### Implicancias

Toda solución deberá considerar:

- desacoplamiento
- extensibilidad
- versionamiento
- modularidad

---

# Ley 6
## Toda arquitectura protege atributos de calidad.

Las funcionalidades entregan valor.

La arquitectura protege ese valor.

Toda decisión debe considerar explícitamente:

- seguridad
- mantenibilidad
- observabilidad
- rendimiento
- resiliencia
- interoperabilidad

No hacerlo constituye una deuda arquitectónica.

---

# Ley 7
## La tecnología nunca es el objetivo.

Las tecnologías son herramientas.

No construimos soluciones alrededor de frameworks.

Construimos soluciones alrededor de problemas.

La tecnología únicamente implementa la arquitectura.

### Está prohibido justificar una decisión con frases como:

- Es tendencia.
- Todo el mundo lo usa.
- Es el framework de moda.
- Lo vi en otra empresa.

---

# Ley 8
## Todo límite debe ser explícito.

Los límites reducen complejidad.

Las responsabilidades deben estar claramente definidas.

Cada componente debe conocer únicamente aquello que necesita conocer.

### Aplica para

- dominios
- APIs
- equipos
- microservicios
- módulos
- repositorios

---

# Ley 9
## La arquitectura debe poder explicarse.

Si una arquitectura necesita una explicación extremadamente compleja probablemente sea demasiado compleja.

Toda solución debe poder comunicarse de forma clara utilizando:

- lenguaje de negocio
- diagramas
- modelos
- documentación

La claridad es un atributo arquitectónico.

---

# Ley 10
## Toda decisión debe ser reversible cuando el contexto cambie.

La arquitectura debe minimizar el costo del cambio.

Ninguna decisión debe convertirse en una prisión tecnológica.

Siempre debemos preguntarnos:

> ¿Qué ocurrirá si dentro de tres años necesitamos reemplazar esta decisión?

---

# Ley 11
## La calidad nunca es negociable.

Las restricciones de tiempo o presupuesto pueden modificar el alcance.

Nunca la calidad fundamental de la arquitectura.

La deuda técnica puede aceptarse.

La deuda arquitectónica debe justificarse.

---

# Ley 12
## El conocimiento es un activo estratégico.

Todo aprendizaje obtenido durante un proyecto debe regresar a la organización.

Aprender sin documentar equivale a perder conocimiento.

### El conocimiento debe transformarse en

- documentación
- estándares
- principios
- ADR
- playbooks
- plantillas

---

# Gobernanza

Toda excepción a una Ley Arquitectónica deberá responder las siguientes preguntas:

## ¿Qué ley será incumplida?

## ¿Por qué?

## ¿Qué riesgo aceptamos?

## ¿Cómo mitigaremos ese riesgo?

## ¿Cuándo será revisada nuevamente?

Las excepciones son temporales.

Las leyes permanecen.

---

# Precedencia

Cuando exista conflicto entre documentos, se aplicará el siguiente orden:

1. Architectural Laws
2. Architectural Principles
3. Architectural Thinking
4. Architectural Decision Model
5. ADR
6. Estándares Técnicos
7. Implementación

Esto garantiza consistencia en todas las decisiones.

---

# Juramento Arquitectónico

Todo arquitecto, desarrollador o consultor que participe en un proyecto de Arquetipo Digital se compromete a:

- Comprender antes de construir.
- Diseñar antes de implementar.
- Documentar antes de olvidar.
- Simplificar antes de complejizar.
- Pensar en la evolución antes que en la entrega inmediata.
- Proteger el conocimiento de la organización.
- Tomar decisiones conscientes y justificables.

---

# Declaración Final

La arquitectura no se mide por la cantidad de componentes, tecnologías o diagramas.

Se mide por la claridad de sus decisiones, la calidad de sus principios y la capacidad del sistema para seguir generando valor cuando el contexto inevitablemente cambie.

---

> **La arquitectura no es lo que construimos.**
>
> **Es la forma en que decidimos construir.**

---

© Arquetipo Digital — Constitutional Document
