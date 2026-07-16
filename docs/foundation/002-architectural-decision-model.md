---
title: Architectural Decision Model
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-16
category: Foundation
---

# Architectural Decision Model (ADM)

> Toda decisión arquitectónica debe ser consciente, justificable y trazable.

---

# Propósito

Este documento define el modelo mediante el cual Arquetipo Digital evalúa, diseña y registra decisiones arquitectónicas.

No pretende reemplazar metodologías como TOGAF, Domain-Driven Design o Clean Architecture.

Su propósito es proporcionar un marco común de razonamiento que permita tomar decisiones consistentes independientemente del proyecto, la tecnología o el dominio de negocio.

Toda decisión importante debe responder primero a este modelo.

---

# Filosofía

Las decisiones arquitectónicas no se toman por intuición.

Tampoco por preferencia tecnológica.

Se toman comprendiendo el problema, evaluando alternativas y analizando sus consecuencias a largo plazo.

La arquitectura consiste en reducir la incertidumbre mediante decisiones conscientes.

---

# El Modelo

Toda decisión debe responder, como mínimo, las siguientes ocho preguntas.

---

# 1. ¿Qué problema estamos resolviendo?

La arquitectura comienza comprendiendo el problema.

No la solución.

Antes de analizar tecnologías debemos responder:

- ¿Cuál es el objetivo?
- ¿Qué necesidad existe?
- ¿Qué resultado esperamos obtener?
- ¿Cuál es el impacto para el negocio?

Si el problema no está claramente definido, ninguna decisión tecnológica tiene sentido.

---

# 2. ¿Cuál es el contexto?

Ninguna decisión existe de manera aislada.

Toda arquitectura depende del contexto.

Debemos comprender:

- organización
- personas
- procesos
- restricciones
- presupuesto
- tiempo
- madurez tecnológica
- capacidades del equipo

Una buena decisión en un contexto puede ser una mala decisión en otro.

---

# 3. ¿Qué alternativas existen?

Nunca diseñamos la primera solución que aparece.

Exploramos alternativas.

Cada alternativa debe ser evaluada considerando:

- simplicidad
- complejidad
- costo
- evolución
- riesgos
- interoperabilidad

La mejor decisión rara vez es la más sofisticada.

Frecuentemente es la más equilibrada.

---

# 4. ¿Cuáles son los atributos de calidad involucrados?

Toda arquitectura debe proteger los atributos de calidad del sistema.

Entre ellos:

- mantenibilidad
- escalabilidad
- disponibilidad
- seguridad
- rendimiento
- resiliencia
- observabilidad
- accesibilidad
- interoperabilidad
- portabilidad

No todos tienen la misma prioridad.

El contexto define cuáles son críticos.

---

# 5. ¿Cuál es el costo del cambio?

Toda decisión genera deuda técnica potencial.

Debemos preguntarnos:

- ¿Qué tan difícil será modificar esta decisión?
- ¿Qué impacto tendrá en cinco años?
- ¿Qué dependencias crea?
- ¿Qué conocimiento requiere mantener?

El costo futuro es tan importante como el beneficio inmediato.

---

# 6. ¿Qué principios estamos reforzando?

Cada decisión debe alinearse con los principios definidos por Arquetipo Digital.

Especialmente:

- claridad
- simplicidad
- desacoplamiento
- evolución
- documentación
- calidad

Si una decisión contradice estos principios, debe justificarse explícitamente.

---

# 7. ¿Cómo validaremos esta decisión?

Toda decisión necesita evidencia.

La validación puede realizarse mediante:

- prototipos
- pruebas técnicas
- métricas
- benchmarking
- pruebas de carga
- revisión arquitectónica
- feedback del negocio

No asumimos.

Validamos.

---

# 8. ¿Cómo documentaremos la decisión?

Una decisión no documentada es una decisión perdida.

Toda decisión relevante debe generar un ADR.

El ADR debe registrar:

- contexto
- decisión
- alternativas
- consecuencias
- fecha
- responsables

El conocimiento pertenece a la organización.

No a las personas.

---

# Flujo de Decisión Arquitectónica

```text
Comprender el problema
          │
          ▼
Analizar el contexto
          │
          ▼
Identificar restricciones
          │
          ▼
Explorar alternativas
          │
          ▼
Evaluar atributos de calidad
          │
          ▼
Analizar impacto y costo del cambio
          │
          ▼
Seleccionar la alternativa
          │
          ▼
Validar
          │
          ▼
Documentar mediante ADR
          │
          ▼
Implementar
          │
          ▼
Medir resultados
          │
          ▼
Aprender y evolucionar
```

---

# Relación con otros marcos

El modelo ADM complementa diferentes metodologías de arquitectura.

| Marco | Cómo se integra |
|--------|-----------------|
| TOGAF | Proporciona gobierno y ciclo de vida de la arquitectura. El ADM guía el razonamiento de cada decisión dentro de ese ciclo. |
| Domain-Driven Design | Ayuda a comprender el dominio y definir límites coherentes. |
| Clean Architecture | Materializa la separación de responsabilidades definida durante el análisis arquitectónico. |
| SOLID | Guía el diseño interno de componentes y clases. |
| C4 Model | Permite comunicar visualmente las decisiones tomadas. |
| ARC42 | Proporciona una estructura para documentar arquitecturas. |
| ADR | Registra formalmente cada decisión arquitectónica. |
| Team Topologies | Orienta la organización de equipos según el flujo de valor. |

Los marcos son herramientas.

El pensamiento arquitectónico permanece.
