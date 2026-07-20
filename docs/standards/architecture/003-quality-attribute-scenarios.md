---
title: Quality Attribute Scenarios
id: ADS-003
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-20
category: Standards
domain: Architecture
references:
  - Architecture Quality Attributes
  - Architecture Review Standard
  - Software Architecture in Practice
  - ISO/IEC 25010
---

# Quality Attribute Scenarios

> Los atributos de calidad no se declaran.
>
> Se demuestran mediante escenarios.

---

# Propósito

Este estándar define cómo Arquetipo Digital especifica, documenta y evalúa atributos de calidad mediante escenarios verificables.

Los escenarios permiten transformar conceptos abstractos como "escalabilidad" o "seguridad" en criterios objetivos para el diseño, revisión y validación de arquitecturas.

Este catálogo constituye una biblioteca reutilizable que puede adaptarse a distintos proyectos y dominios.

---

# Filosofía

Decir que un sistema debe ser "seguro", "rápido" o "escalable" no es suficiente.

Todo atributo de calidad debe responder:

- ¿Qué ocurre?
- ¿Cuándo ocurre?
- ¿Qué debe hacer el sistema?
- ¿Cómo sabremos que lo logró?

---

# Estructura oficial

Todo escenario debe seguir el siguiente formato.

| Campo | Descripción |
|--------|-------------|
| ID | Identificador único |
| Atributo | Calidad evaluada |
| Fuente | Actor o evento que inicia el escenario |
| Estímulo | Situación que ocurre |
| Contexto | Condiciones en las que sucede |
| Respuesta esperada | Comportamiento esperado |
| Medición | Cómo se verifica |

---

# Escalabilidad

## QAS-001

### Atributo

Escalabilidad

### Fuente

Usuarios

### Estímulo

El tráfico aumenta un 300% durante una campaña.

### Contexto

Horario de mayor demanda.

### Respuesta esperada

La plataforma continúa respondiendo sin degradar la experiencia.

### Medición

- Tiempo de respuesta < 2 segundos.
- Disponibilidad ≥ 99.9%.
- Sin pérdida de solicitudes.

---

## QAS-002

### Atributo

Escalabilidad

### Estímulo

Se incorpora un nuevo módulo funcional.

### Respuesta esperada

Puede desplegarse sin modificar componentes existentes.

### Medición

- Sin interrupción del servicio.
- Sin cambios en módulos no relacionados.

---

# Rendimiento

## QAS-010

### Atributo

Rendimiento

### Estímulo

Un usuario consulta información.

### Contexto

Operación normal.

### Respuesta esperada

La información se entrega oportunamente.

### Medición

95% de las consultas en menos de 500 ms.

---

## QAS-011

### Estímulo

Carga masiva de datos.

### Respuesta esperada

El procesamiento mantiene tiempos aceptables.

### Medición

Procesamiento completo en menos de 10 minutos para 1 millón de registros.

---

# Seguridad

## QAS-020

### Estímulo

Intento de acceso no autorizado.

### Respuesta esperada

El acceso es rechazado y registrado.

### Medición

- Acceso denegado.
- Evento auditado.
- Alerta generada.

---

## QAS-021

### Estímulo

Compromiso de credenciales.

### Respuesta esperada

La sesión es invalidada automáticamente.

### Medición

Tiempo de revocación < 60 segundos.

---

# Observabilidad

## QAS-030

### Estímulo

Falla en una transacción crítica.

### Respuesta esperada

La causa puede identificarse mediante trazabilidad completa.

### Medición

100% de las transacciones poseen un identificador único.

---

## QAS-031

### Estímulo

Error inesperado.

### Respuesta esperada

Logs estructurados disponibles.

### Medición

Todos los errores contienen:

- Correlation ID
- Timestamp
- Servicio
- Severidad

---

# Resiliencia

## QAS-040

### Estímulo

Caída de una instancia.

### Respuesta esperada

El servicio continúa funcionando.

### Medición

Recuperación automática en menos de 60 segundos.

---

## QAS-041

### Estímulo

Falla de un servicio externo.

### Respuesta esperada

El sistema degrada funcionalidades de manera controlada.

### Medición

No se produce indisponibilidad total.

---

# Mantenibilidad

## QAS-050

### Estímulo

Cambio en una regla de negocio.

### Respuesta esperada

Puede implementarse sin afectar otros módulos.

### Medición

No requiere modificaciones fuera del dominio correspondiente.

---

## QAS-051

### Estímulo

Ingreso de un nuevo desarrollador.

### Respuesta esperada

Puede comprender la arquitectura rápidamente.

### Medición

Onboarding técnico completado en menos de cinco días.

---

# Interoperabilidad

## QAS-060

### Estímulo

Integración con un nuevo sistema.

### Respuesta esperada

Se implementa mediante interfaces existentes.

### Medición

No requiere modificar consumidores actuales.

---

# Disponibilidad

## QAS-070

### Estímulo

Falla de infraestructura.

### Respuesta esperada

El servicio permanece disponible.

### Medición

Disponibilidad anual ≥ 99.95%.

---

# Evolución

## QAS-080

### Estímulo

Nueva funcionalidad.

### Respuesta esperada

Puede incorporarse sin reescribir la arquitectura.

### Medición

El cambio reutiliza componentes existentes.

---

# Accesibilidad

## QAS-090

### Estímulo

Uso mediante lector de pantalla.

### Respuesta esperada

La interfaz es completamente navegable.

### Medición

Cumplimiento WCAG 2.2 AA.

---

# Adaptabilidad

## QAS-100

### Estímulo

Cambio regulatorio.

### Respuesta esperada

La solución incorpora la nueva normativa sin afectar otros procesos.

### Medición

Cambios aislados y trazables.

---

# Cómo seleccionar escenarios

No todos los escenarios aplican a todos los proyectos.

Cada iniciativa debe identificar:

- atributos críticos;
- escenarios relevantes;
- métricas de aceptación.

---

# Matriz de priorización

| Tipo de proyecto | Atributos prioritarios |
|------------------|------------------------|
| Landing corporativa | Rendimiento · Accesibilidad · Disponibilidad |
| API | Rendimiento · Seguridad · Observabilidad |
| SaaS | Escalabilidad · Resiliencia · Observabilidad |
| Integración | Interoperabilidad · Disponibilidad · Seguridad |
| IA Generativa | Observabilidad · Seguridad · Evolución |
| Arquitectura Empresarial | Adaptabilidad · Evolución · Mantenibilidad |

---

# Uso durante ARCHE

| Etapa | Uso |
|--------|-----|
| Analyze | Identificar atributos críticos del negocio |
| Reason | Comparar alternativas según escenarios |
| Create | Diseñar mecanismos que satisfagan los escenarios |
| Harmonize | Verificar cumplimiento durante la revisión |
| Evolve | Medir resultados y ajustar escenarios |

---

# Buenas prácticas

✔ Escribir escenarios verificables.

✔ Definir métricas objetivas.

✔ Asociar cada escenario a un atributo de calidad.

✔ Priorizar según el contexto del negocio.

✔ Revisar periódicamente los escenarios.

---

# Antipatrones

Evitar expresiones como:

- "El sistema debe ser rápido."
- "La plataforma debe ser segura."
- "La aplicación debe ser escalable."

Estas afirmaciones no pueden validarse.

Siempre deben transformarse en escenarios medibles.

---

# Declaración Final

Los atributos de calidad no representan aspiraciones.

Representan compromisos medibles que orientan las decisiones arquitectónicas y permiten evaluar objetivamente si una solución cumple con las necesidades del negocio.

Cada escenario es una hipótesis verificable sobre el comportamiento esperado del sistema.

---

> **Una arquitectura madura no promete calidad.**
>
> **La especifica, la mide y la demuestra.**

---

© Arquetipo Digital — Architecture Standards
