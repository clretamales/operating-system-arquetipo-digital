---
title: Architecture Decision Standard
id: ADS-004
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-20
category: Standards
domain: Architecture
framework: ARCHE
references:
  - Architectural Decision Model
  - Architecture Review Standard
  - Architecture Quality Attributes
  - Architectural Principles Catalog
  - Architectural Laws
---

# Architecture Decision Standard

> Una decisión arquitectónica no se define por su complejidad.
>
> Se define por el impacto que tendrá sobre la evolución del sistema.

---

# Propósito

Este estándar establece cómo Arquetipo Digital identifica, analiza, aprueba, documenta y gobierna las decisiones arquitectónicas.

Su objetivo es garantizar que las decisiones más importantes sean conscientes, trazables, justificables y revisables.

No todas las decisiones requieren un registro formal.

Este estándar ayuda a distinguir entre una decisión técnica cotidiana y una verdadera decisión arquitectónica.

---

# Filosofía

Toda arquitectura es el resultado de una secuencia de decisiones.

Los diagramas representan esas decisiones.

El software implementa esas decisiones.

La documentación preserva esas decisiones.

Por ello, la calidad de una arquitectura depende directamente de la calidad de las decisiones que la originaron.

---

# ¿Qué es una decisión arquitectónica?

Una decisión arquitectónica es aquella que modifica de manera significativa uno o más de los siguientes aspectos:

- estructura del sistema;
- atributos de calidad;
- evolución futura;
- costos operacionales;
- experiencia del usuario;
- integración con otros sistemas;
- riesgos del negocio.

Si una decisión puede afectar la arquitectura durante meses o años, debe tratarse como una decisión arquitectónica.

---

# ¿Qué NO es una decisión arquitectónica?

Normalmente no requieren un ADR:

- elección de nombres de variables;
- estructura de carpetas;
- estilos de código;
- configuración de IDE;
- cambios cosméticos;
- refactorizaciones sin impacto arquitectónico.

Estas decisiones se gobiernan mediante estándares técnicos y revisiones de código.

---

# Criterios de identificación

Antes de registrar una decisión, responder las siguientes preguntas.

| Pregunta | Sí | No |
|-----------|:--:|:--:|
| ¿Impacta la arquitectura? | □ | □ |
| ¿Impacta atributos de calidad? | □ | □ |
| ¿Genera deuda arquitectónica si cambia? | □ | □ |
| ¿Tiene consecuencias de largo plazo? | □ | □ |
| ¿Existen alternativas relevantes? | □ | □ |

Si la mayoría de las respuestas es afirmativa, la decisión debe tratarse como arquitectónica.

---

# Modelo de decisión

Toda decisión sigue el siguiente flujo.

```text
Problema

↓

Contexto

↓

Alternativas

↓

Evaluación

↓

Decisión

↓

ADR

↓

Revisión

↓

Implementación

↓

Aprendizaje
```

Ninguna decisión importante debe omitir etapas.

---

# Evidencia mínima

Antes de aprobar una decisión debe existir evidencia suficiente.

## Contexto

¿Qué problema se intenta resolver?

---

## Restricciones

¿Qué limita las alternativas?

---

## Objetivos

¿Qué buscamos optimizar?

---

## Riesgos

¿Qué riesgos aceptamos?

---

## Alternativas

¿Qué otras opciones fueron consideradas?

---

## Consecuencias

¿Qué cambia si adoptamos esta decisión?

---

# Relación con ARCHE

Las decisiones se generan principalmente durante la etapa **Reason**, se formalizan en **Create**, se validan en **Harmonize** y se revisan continuamente durante **Evolve**.

| Etapa | Rol |
|--------|-----|
| Analyze | Comprender el problema |
| Reason | Evaluar alternativas |
| Create | Formalizar la decisión |
| Harmonize | Revisar y aprobar |
| Evolve | Revaluar y actualizar |

---

# Relación con atributos de calidad

Toda decisión debe indicar explícitamente qué atributos fortalece o compromete.

Ejemplo:

| Atributo | Impacto |
|----------|---------|
| Seguridad | Alto |
| Escalabilidad | Medio |
| Rendimiento | Bajo |
| Observabilidad | Alto |

Toda decisión implica compromisos.

Estos deben hacerse visibles.

---

# Relación con principios

Toda decisión debe indicar qué principios arquitectónicos aplica.

Ejemplo

- AP-001 El contexto precede a la tecnología.
- AP-004 La simplicidad es una decisión arquitectónica.
- AP-007 La calidad es responsabilidad de la arquitectura.

---

# Relación con las Leyes Arquitectónicas

Ninguna decisión puede contradecir una Ley Arquitectónica sin una excepción formal.

Las excepciones deben:

- documentarse;
- justificarse;
- aprobarse;
- revisarse periódicamente.

---

# Clasificación de decisiones

Las decisiones pueden clasificarse según su alcance.

| Nivel | Ejemplo |
|--------|----------|
| Estratégica | Arquitectura empresarial, plataforma, cloud |
| Táctica | Patrón de integración, autenticación |
| Operativa | Herramientas de observabilidad, CI/CD |

Esta clasificación ayuda a determinar el nivel de revisión requerido.

---

# Estados

Toda decisión posee un ciclo de vida.

| Estado | Descripción |
|----------|-------------|
| Proposed | En análisis |
| Accepted | Aprobada |
| Implemented | Implementada |
| Superseded | Reemplazada |
| Deprecated | No recomendada |
| Archived | Histórica |

Las decisiones nunca desaparecen.

Evolucionan.

---

# Criterios de aprobación

Una decisión puede aprobarse cuando:

- el problema está claramente definido;
- existen alternativas evaluadas;
- los riesgos son conocidos;
- los atributos de calidad fueron considerados;
- la decisión está alineada con los principios;
- cumple las Leyes Arquitectónicas.

---

# Checklist

## Problema

□ Existe evidencia del problema.

---

## Contexto

□ Restricciones identificadas.

□ Objetivos claros.

---

## Alternativas

□ Existen al menos dos alternativas evaluadas (cuando sea razonable).

□ Trade-offs documentados.

---

## Calidad

□ Atributos evaluados.

□ Riesgos registrados.

---

## Gobernanza

□ Principios aplicados.

□ Leyes verificadas.

□ ADR preparado.

---

# Cuándo crear un ADR

Debe generarse un ADR cuando la decisión:

- modifica la arquitectura;
- afecta múltiples equipos;
- introduce una nueva plataforma;
- cambia atributos de calidad;
- genera deuda arquitectónica;
- altera contratos públicos;
- impacta el modelo operativo.

No documentar estas decisiones dificulta la evolución futura.

---

# Antipatrones

Evitar decisiones basadas únicamente en:

- preferencias personales;
- tecnologías de moda;
- autoridad jerárquica;
- experiencia aislada;
- "siempre lo hemos hecho así".

Toda decisión debe sustentarse en evidencia.

---

# Métricas

El proceso debe medir:

- decisiones registradas;
- ADR creados;
- decisiones reemplazadas;
- tiempo promedio de aprobación;
- excepciones activas;
- decisiones revisadas;
- decisiones sin evidencia suficiente.

Estas métricas alimentan la mejora continua del Framework ARCHE.

---

# Relación con otros estándares

Este estándar complementa:

- Architecture Document Standard
- Architecture Review Standard
- Quality Attribute Scenarios
- Architectural Decision Model
- Architectural Principles Catalog
- Architectural Laws

---

# Declaración Final

Una arquitectura sostenible no depende únicamente de buenas decisiones.

Depende de decisiones que puedan comprenderse, cuestionarse, justificarse y evolucionar con el tiempo.

Cada decisión arquitectónica representa una inversión en el futuro del sistema.

Por ello, decidir con evidencia es tan importante como implementar correctamente.

---

> **La arquitectura no es la suma de sus componentes.**
>
> **Es la suma de las decisiones que permanecen cuando los componentes cambian.**

---

© Arquetipo Digital — Architecture Standards
