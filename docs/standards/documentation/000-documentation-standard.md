---
title: Documentation Standard
id: DOC-000
version: 1.0
status: Official
owner: Arquetipo Digital
last_updated: 2026-07-20
category: Standards
domain: Documentation
framework: ARCHE
references:
  - Architecture Document Standard
  - Architecture Playbook
  - Architectural Laws
  - Architecture Governance Standard
---

# Documentation Standard

> La documentación no existe para registrar el pasado.
>
> Existe para permitir el futuro.

---

# Propósito

Este estándar define cómo Arquetipo Digital crea, organiza, mantiene y evoluciona toda su documentación.

La documentación constituye uno de los principales activos intelectuales de la organización.

No representa un entregable adicional.

Forma parte del producto.

Forma parte de la arquitectura.

Forma parte del conocimiento organizacional.

---

# Filosofía

Las personas cambian.

Los equipos cambian.

Las tecnologías cambian.

La documentación debe permitir que el conocimiento permanezca.

Nuestro objetivo no es escribir más documentos.

Nuestro objetivo es reducir incertidumbre.

---

# Principios

Toda documentación producida por Arquetipo Digital debe cumplir los siguientes principios.

---

## 1. Escribir para la siguiente persona

Toda documentación debe responder una pregunta.

Nunca debe escribirse únicamente para quien la creó.

---

## 2. La documentación pertenece al proyecto

Nunca pertenece a un individuo.

La organización es propietaria del conocimiento.

---

## 3. Documentar decisiones

No describimos únicamente resultados.

Documentamos:

- por qué;
- cómo;
- qué alternativas existían;
- qué riesgos aceptamos.

---

## 4. Mantener una única fuente de verdad

Cada conocimiento debe tener un único lugar oficial.

Evitar duplicar contenido.

Cuando un documento depende de otro, debe referenciarlo.

---

## 5. Evolucionar continuamente

La documentación nunca está terminada.

Debe evolucionar junto con la arquitectura.

---

# Tipos de documentación

Toda documentación pertenece a una de las siguientes categorías.

| Categoría | Objetivo |
|-----------|----------|
| Foundation | Filosofía, principios y metodología |
| Standards | Normas oficiales |
| Playbooks | Procedimientos operativos |
| ADR | Decisiones arquitectónicas |
| RFC | Propuestas de cambio |
| Knowledge | Conocimiento reutilizable |
| Guides | Guías prácticas |
| Tutorials | Aprendizaje paso a paso |
| Reference | Información de consulta |
| Runbooks | Operación e incidentes |

Cada documento debe pertenecer únicamente a una categoría.

---

# Estructura mínima

Todo documento debe contener.

```yaml
title:
id:
version:
status:
owner:
category:
domain:
references:
last_review:
next_review:
```

Esto permite gobernanza documental.

---

# Estados

Todo documento posee un ciclo de vida.

| Estado | Descripción |
|----------|-------------|
| Draft | En elaboración |
| Review | En revisión |
| Approved | Vigente |
| Deprecated | En retirada |
| Archived | Histórico |

Nunca eliminar documentos históricos.

El conocimiento también tiene historia.

---

# Versionado

Aplicamos versionado semántico.

| Versión | Uso |
|----------|-----|
| 1.0 | Primera versión oficial |
| 1.1 | Correcciones menores |
| 1.2 | Mejoras incrementales |
| 2.0 | Cambio estructural importante |

Toda modificación significativa debe registrarse.

---

# Estructura recomendada

Todo documento debe seguir un flujo lógico.

```text
Propósito

↓

Contexto

↓

Contenido

↓

Ejemplos

↓

Buenas prácticas

↓

Antipatrones

↓

Referencias

↓

Declaración Final
```

La estructura puede adaptarse según el tipo de documento.

---

# Estilo de escritura

Toda documentación debe ser:

- clara;
- objetiva;
- concisa;
- consistente;
- verificable.

Evitar:

- ambigüedad;
- opiniones sin evidencia;
- lenguaje innecesariamente complejo;
- tecnicismos cuando no aportan valor.

---

# Convenciones

Utilizar:

- títulos descriptivos;
- listas cuando mejoren la comprensión;
- tablas para comparar información;
- diagramas cuando reduzcan complejidad;
- ejemplos reales.

Evitar bloques extensos de texto cuando una estructura visual sea más efectiva.

---

# Referencias cruzadas

La documentación forma una red de conocimiento.

Siempre que exista una dependencia, debe referenciarse el documento correspondiente.

Ejemplo.

```text
Este estándar complementa:

ADS-000

ADS-001

DOC-002
```

Nunca copiar contenido completo entre documentos.

---

# Diagramas

Todo diagrama debe:

- responder una pregunta;
- tener un propósito;
- indicar su versión;
- mantenerse sincronizado con la arquitectura.

Los diagramas son documentación.

No ilustraciones.

---

# Calidad documental

Antes de aprobar un documento verificar.

□ Existe un propósito claro.

□ Existe contexto suficiente.

□ La información es verificable.

□ No existen contradicciones.

□ Se encuentran definidas las responsabilidades.

□ Se referencian documentos relacionados.

□ Se encuentran identificados los riesgos cuando corresponde.

□ Está escrito para una audiencia claramente definida.

---

# Responsabilidades

## Autor

Escribe el documento.

Mantiene su contenido.

---

## Reviewer

Verifica claridad.

Consistencia.

Exactitud.

---

## Owner

Aprueba.

Prioriza.

Garantiza vigencia.

---

## Consumer

Utiliza el conocimiento.

Retroalimenta mejoras.

---

# Frecuencia de revisión

Todo documento debe revisarse periódicamente.

| Tipo | Frecuencia |
|--------|------------|
| Foundation | Anual |
| Standards | Semestral |
| ADR | Cuando cambie el contexto |
| Runbooks | Trimestral |
| Playbooks | Semestral |
| Guías | Según necesidad |

---

# Gestión del conocimiento

El conocimiento evoluciona siguiendo este ciclo.

```text
Experiencia

↓

Aprendizaje

↓

Documentación

↓

Compartir

↓

Aplicar

↓

Mejorar

↓

Nuevo conocimiento
```

La documentación transforma experiencia individual en conocimiento organizacional.

---

# Antipatrones

Evitar:

- documentación duplicada;
- documentación desactualizada;
- documentos sin responsable;
- documentos sin propósito;
- conocimiento únicamente verbal;
- documentación escrita al final del proyecto.

---

# Definition of Done

Un documento está completo cuando:

- responde el problema que motivó su creación;
- puede comprenderse sin ayuda del autor;
- posee responsable;
- posee versión;
- posee referencias;
- está alineado con los estándares;
- agrega valor al conocimiento organizacional.

---

# Relación con ARCHE

| Etapa | Rol de la documentación |
|--------|--------------------------|
| Analyze | Registrar contexto y descubrimientos |
| Reason | Justificar decisiones y alternativas |
| Create | Documentar arquitectura y modelos |
| Harmonize | Respaldar revisiones y aprobaciones |
| Evolve | Preservar aprendizajes y mejoras |

La documentación acompaña todo el ciclo de vida.

---

# Declaración Final

Para Arquetipo Digital, documentar no significa producir archivos.

Significa preservar conocimiento.

Cada documento representa una inversión para que las futuras decisiones sean mejores, más rápidas y menos dependientes de personas específicas.

La documentación es la memoria institucional de la arquitectura.

---

> **El conocimiento que no se documenta se pierde.**
>
> **El conocimiento bien documentado se convierte en una ventaja competitiva.**

---

© Arquetipo Digital — Documentation Standards
