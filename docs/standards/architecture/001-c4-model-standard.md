---
title: C4 Model Standard
id: ADS-001
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-20
category: Standards
domain: Architecture
references:
  - Architecture Document Standard
  - ARCHE Framework
  - Simon Brown - C4 Model
---

# C4 Model Standard

> Un diagrama no existe para mostrar una arquitectura.
>
> Existe para responder una pregunta.

---

# Propósito

Este estándar define cómo Arquetipo Digital utiliza el modelo **C4** para comunicar arquitecturas de manera clara, consistente y orientada al contexto.

No establece reglas de dibujo.

Establece reglas de comunicación.

Nuestro objetivo no es producir diagramas.

Nuestro objetivo es reducir incertidumbre.

---

# Filosofía

Todo diagrama debe responder una pregunta específica.

Si un diagrama no responde una pregunta concreta, no debe existir.

Preferimos pocos diagramas útiles antes que muchos diagramas innecesarios.

---

# Principios

Toda representación arquitectónica debe cumplir los siguientes principios.

## Claridad

Debe comprenderse en pocos minutos.

---

## Contexto

Debe mostrar únicamente la información necesaria.

---

## Simplicidad

Eliminar elementos irrelevantes.

---

## Consistencia

Todos los proyectos utilizan la misma notación.

---

## Evolución

Los diagramas evolucionan junto con la arquitectura.

Nunca son fotografías permanentes.

---

# El Modelo C4

El modelo C4 organiza una arquitectura en cuatro niveles de abstracción.

```text
System Context

↓

Containers

↓

Components

↓

Code
```

Cada nivel responde una pregunta distinta.

---

# Nivel 1 — System Context

## Pregunta

¿Qué sistema estamos construyendo y cómo se relaciona con su entorno?

---

## Objetivo

Comprender el sistema desde la perspectiva del negocio.

---

## Debe incluir

- Sistema principal
- Usuarios
- Sistemas externos
- Relaciones
- Flujos principales

---

## No debe incluir

- Bases de datos
- APIs internas
- Frameworks
- Infraestructura
- Clases

---

## Audiencia

- Negocio
- Arquitectos
- Product Owners
- Stakeholders

---

# Nivel 2 — Container Diagram

## Pregunta

¿Cómo está organizado internamente el sistema?

---

## Objetivo

Mostrar los grandes bloques tecnológicos.

---

## Puede incluir

- Frontend
- Backend
- API
- Base de Datos
- Cola
- Cache
- Servicios

---

## No debe incluir

- Clases
- Métodos
- Código

---

## Audiencia

- Arquitectos
- Líderes técnicos
- Desarrolladores

---

# Nivel 3 — Component Diagram

## Pregunta

¿Cómo se organiza un contenedor?

---

## Objetivo

Mostrar responsabilidades internas.

---

## Incluye

- Componentes
- Interfaces
- Dependencias
- Responsabilidades

---

## No incluye

- Código
- Métodos privados
- Implementación

---

## Audiencia

Equipos de desarrollo.

---

# Nivel 4 — Code Diagram

## Pregunta

¿Cómo implementamos un componente?

---

## Objetivo

Documentar estructuras complejas cuando realmente agregan valor.

---

## Recomendación

Evitar documentar automáticamente todo el código.

Solo crear esta vista cuando facilite la comprensión.

---

# ¿Cuándo utilizar cada nivel?

| Tipo de proyecto | Context | Containers | Components | Code |
|------------------|:------:|:----------:|:----------:|:----:|
| Landing Page | ✔ | ○ | ✖ | ✖ |
| API REST | ✔ | ✔ | ✔ | ○ |
| Microservicios | ✔ | ✔ | ✔ | ○ |
| Plataforma SaaS | ✔ | ✔ | ✔ | ○ |
| Arquitectura Empresarial | ✔ | ✔ | ○ | ✖ |
| IA Generativa | ✔ | ✔ | ✔ | ○ |

✔ Obligatorio

○ Opcional

✖ No recomendado

---

# Convenciones

Todos los diagramas deben utilizar nombres consistentes.

Ejemplo

```text
Customer Portal

Orders API

Identity Service

Payments Database
```

Evitar nombres como:

```text
Sistema 1

Servicio Nuevo

Backend

API2
```

Los nombres deben describir responsabilidades.

---

# Relaciones

Todas las relaciones deben indicar:

- Dirección
- Tipo de comunicación
- Protocolo (cuando sea relevante)

Ejemplo

```text
Frontend

↓

HTTPS

↓

Orders API
```

---

# Colores

Los colores representan categorías.

| Categoría | Uso |
|-----------|-----|
| Azul | Aplicaciones |
| Verde | Sistemas externos |
| Gris | Infraestructura |
| Naranja | Bases de datos |
| Morado | Servicios compartidos |

Los colores nunca representan importancia.

---

# Nivel de detalle

Aplicamos la regla:

**Una vista = un nivel de abstracción.**

Nunca mezclar:

- Contexto
- Contenedores
- Componentes
- Código

En un mismo diagrama.

---

# Antipatrones

No hacer diagramas con:

- exceso de texto;
- todas las clases del sistema;
- cada endpoint;
- cada tabla;
- cada servidor;
- cada dependencia técnica.

Más detalle no significa mejor arquitectura.

---

# Buenas prácticas

✔ Un propósito por diagrama.

✔ Un nivel de abstracción.

✔ Lenguaje del negocio cuando sea posible.

✔ Nombres consistentes.

✔ Relaciones explícitas.

✔ Diagramas fáciles de actualizar.

---

# Relación con ARCHE

| Etapa | Uso del C4 |
|--------|------------|
| Analyze | Context Diagram |
| Reason | Context + Alternativas |
| Create | Context + Containers + Components |
| Harmonize | Validación de vistas |
| Evolve | Actualización de diagramas |

El modelo C4 acompaña todo el ciclo de vida del proyecto.

---

# Checklist

Antes de publicar un diagrama verificar:

□ Tiene un propósito claro.

□ Responde una pregunta.

□ Utiliza el nivel correcto.

□ Elimina detalles innecesarios.

□ Los nombres son consistentes.

□ Las relaciones están identificadas.

□ Puede comprenderse sin explicación verbal.

---

# Declaración Final

En Arquetipo Digital no dibujamos diagramas para documentar sistemas.

Los utilizamos para facilitar decisiones, comunicar conocimiento y reducir la complejidad.

Cada vista arquitectónica debe aportar claridad.

Si un diagrama no mejora la comprensión del sistema, no debe formar parte de la arquitectura.

---

> **Un buen diagrama no muestra todo.**
>
> **Muestra exactamente lo necesario para tomar una mejor decisión.**

---

© Arquetipo Digital — Architecture Standards
