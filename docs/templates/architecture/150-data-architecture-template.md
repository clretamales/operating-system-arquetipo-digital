---
title: <Arquitectura de Datos>
id: ARC-DAT-150
version: 1.0
status: Draft
owner: Arquetipo Digital
category: Architecture
type: Data Architecture
domain: Data
framework: ARCHE
classification: Logical
authors:
  - <Autor>
reviewers:
  - <Revisor>
approvers:
  - <Aprobador>
created: YYYY-MM-DD
last_updated: YYYY-MM-DD
next_review: YYYY-MM-DD
references:
  - ARC-EA-120 Enterprise Architecture
  - ARC-SOL-100 Solution Architecture
  - ARC-SW-110 Software Architecture
  - ARC-INT-140 Integration Architecture
  - ADS-004 Architecture Decision Standard
tags:
  - architecture
  - data
---

# Arquitectura de Datos

> Los datos no son únicamente información.

> Representan el conocimiento operacional de una organización.

---

# Resumen Ejecutivo

Describir:

- necesidad del negocio;
- estrategia de datos;
- beneficios esperados;
- principales riesgos;
- objetivos de gobernanza.

---

# Información General

| Campo | Valor |
|--------|-------|
| Proyecto | |
| Organización | |
| Dominio | |
| Arquitecto de Datos | |
| Estado | |
| Versión | |

---

# Contexto

## Problema

¿Qué problema de negocio motiva esta arquitectura?

---

## Objetivos

### Negocio

-

### Datos

-

### Analítica

-

### Gobierno

-

---

# Alcance

## Incluye

-

## Excluye

-

## Restricciones

-

## Supuestos

-

---

# Dominios de Datos

Identificar los dominios principales.

| Dominio | Responsable |
|----------|-------------|
| Clientes | |
| Productos | |
| Consentimientos | |
| Facturación | |

Cuando aplique, utilizar Domain Driven Design.

---

# Conceptos del Negocio

Documentar los conceptos fundamentales.

| Concepto | Definición |
|-----------|------------|
| Cliente | |
| Orden | |
| Consentimiento | |

Evitar definir tablas.

Definir conceptos.

---

# Modelo Conceptual

Agregar diagrama conceptual.

Mostrar únicamente relaciones de negocio.

---

# Modelo Lógico

Documentar:

- entidades;
- atributos;
- relaciones;
- cardinalidades.

---

# Modelo Físico

Documentar:

- motores de base de datos;
- particiones;
- índices;
- almacenamiento.

---

# Arquitectura de Persistencia

## Bases de Datos

| Tecnología | Uso |
|-------------|-----|
| SQL Server | |
| PostgreSQL | |
| Oracle | |
| MongoDB | |

Justificar la elección.

---

## Caché

Documentar.

- Redis
- Memoria
- CDN

---

## Data Lake

Cuando corresponda.

---

## Data Warehouse

Cuando corresponda.

---

# Flujo de Datos

Agregar diagrama.

```text
Origen

↓

Captura

↓

Transformación

↓

Persistencia

↓

Consumo
```

---

# Integración de Datos

Documentar.

- ETL
- ELT
- CDC
- Streaming
- Batch
- APIs
- Eventos

---

# Calidad de Datos

Definir criterios.

| Dimensión | Objetivo |
|------------|----------|
| Exactitud | |
| Integridad | |
| Consistencia | |
| Oportunidad | |
| Unicidad | |

---

# Datos Maestros (MDM)

Cuando aplique.

Documentar:

- entidades maestras;
- golden record;
- sincronización;
- reconciliación.

---

# Metadata

Documentar.

- catálogo;
- diccionario;
- linaje;
- clasificación.

---

# Linaje de Datos

Documentar el recorrido de la información.

```text
Origen

↓

Transformación

↓

Persistencia

↓

API

↓

Dashboard

↓

Usuario
```

---

# Seguridad

Documentar.

## Clasificación

| Tipo | Ejemplo |
|------|----------|
| Pública | |
| Interna | |
| Confidencial | |
| Sensible | |

---

## Protección

- cifrado;
- anonimización;
- enmascaramiento;
- tokenización.

---

## Cumplimiento

- GDPR
- ISO 27001
- PCI DSS
- HIPAA
- Leyes locales

---

# Analítica

Documentar.

- BI
- Dashboards
- KPIs
- IA
- Machine Learning

---

# Retención

Definir políticas.

| Tipo | Tiempo |
|------|---------|
| Operacional | |
| Auditoría | |
| Histórico | |

---

# Eliminación

Documentar políticas de:

- borrado;
- archivado;
- anonimización.

---

# Atributos de Calidad

| Atributo | Prioridad | Estrategia |
|----------|-----------|------------|
| Calidad | Alta | |
| Disponibilidad | Alta | |
| Integridad | Alta | |
| Seguridad | Alta | |
| Escalabilidad | Media | |

---

# Riesgos

| Riesgo | Mitigación |
|----------|------------|
| Riesgo | |

---

# ADR Relacionados

Referenciar decisiones.

---

# Roadmap

```text
Modelo Conceptual

↓

Modelo Lógico

↓

Persistencia

↓

Gobierno

↓

Analítica

↓

Optimización
```

---

# Checklist

## Modelado

- [ ] Dominios definidos
- [ ] Modelo conceptual
- [ ] Modelo lógico
- [ ] Modelo físico

---

## Calidad

- [ ] Calidad definida
- [ ] Linaje documentado
- [ ] Catálogo actualizado

---

## Seguridad

- [ ] Clasificación
- [ ] Cifrado
- [ ] Retención

---

## Gobernanza

- [ ] Propietarios definidos
- [ ] Políticas documentadas
- [ ] ADR registrados

---

# Documentos Relacionados

- Enterprise Architecture
- Solution Architecture
- Software Architecture
- Integration Architecture
- Security Architecture
- Data Governance
- ADR

---

# Historial

| Versión | Fecha | Descripción |
|----------|------|-------------|
| 1.0 | YYYY-MM-DD | Primera versión |

---

# Aprobaciones

| Rol | Responsable | Fecha |
|------|-------------|------|
| Data Architect | | |
| Data Owner | | |
| Enterprise Architect | | |

---

# Declaración Final

La Arquitectura de Datos establece cómo una organización organiza, protege, comparte y utiliza la información como un activo estratégico.

Su propósito no es únicamente definir tecnologías de almacenamiento, sino proporcionar un modelo coherente que garantice calidad, trazabilidad, seguridad y reutilización de los datos durante todo su ciclo de vida.

---

> **Las aplicaciones consumen datos.**
>
> **El negocio genera significado.**
>
> **La Arquitectura de Datos conecta ambos mundos.**

---

© Arquetipo Digital
