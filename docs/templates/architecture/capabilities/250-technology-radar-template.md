---
title: <Technology Radar>
id: ARC-RAD-250
version: 1.0
status: Draft
owner: Arquetipo Digital
category: Architecture
type: Technology Radar
domain: Technology
framework: ARCHE
classification: Governance
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
  - ARC-GOV-200 Governance Architecture
  - ARC-SUS-240 Sustainability Architecture
  - ADS-004 Architecture Decision Standard
tags:
  - technology
  - radar
  - governance
---

# Technology Radar

> Las tecnologías cambian constantemente.
>
> Los principios arquitectónicos deben permanecer.

El Technology Radar de ARCHE permite evaluar, priorizar y gobernar la adopción de tecnologías alineándolas con la estrategia del negocio y la evolución de la arquitectura.

---

# Resumen Ejecutivo

Describir:

- estado tecnológico actual;
- tecnologías estratégicas;
- tecnologías en evaluación;
- tecnologías en retiro;
- principales riesgos.

---

# Información General

| Campo | Valor |
|--------|-------|
| Organización | |
| Arquitecto Responsable | |
| Periodo | |
| Estado | |
| Versión | |

---

# Objetivo

Responder:

- ¿Qué tecnologías promovemos?
- ¿Cuáles restringimos?
- ¿Cuáles retiraremos?
- ¿Qué riesgos existen?
- ¿Cómo evolucionará el ecosistema?

---

# Principios

El radar debe cumplir los siguientes principios.

- El negocio impulsa la tecnología.
- Las decisiones deben ser trazables.
- La innovación debe ser controlada.
- La estandarización reduce complejidad.
- La obsolescencia debe gestionarse.

---

# Categorías

Clasificar tecnologías.

## Lenguajes

Ejemplo.

- C#
- Java
- Go
- Python

---

## Frameworks

- ASP.NET Core
- Spring
- Node.js

---

## Frontend

- Web Components
- Blazor
- Angular

---

## Bases de Datos

- SQL Server
- PostgreSQL
- Oracle
- MongoDB

---

## Integración

- RabbitMQ
- Kafka
- Azure Service Bus

---

## Cloud

- Azure
- AWS
- GCP

---

## DevOps

- GitHub Actions
- Azure DevOps
- Terraform
- Bicep

---

## Observabilidad

- OpenTelemetry
- Prometheus
- Grafana
- New Relic

---

## IA

- Semantic Kernel
- LangChain
- MCP
- OpenAI
- Ollama

---

## Seguridad

- OAuth2
- OIDC
- Keycloak
- Microsoft Entra ID

---

# Estados del Radar

Cada tecnología debe tener un estado.

## Adoptar

Uso recomendado.

Tecnología madura y aprobada.

---

## Probar

Puede utilizarse en proyectos controlados.

Debe existir seguimiento.

---

## Evaluar

Existe interés.

Aún no existe recomendación oficial.

---

## Restringir

No se recomienda para nuevos desarrollos.

Puede mantenerse en sistemas existentes.

---

## Retirar

Debe planificarse su eliminación.

No debe utilizarse en nuevos proyectos.

---

# Catálogo Tecnológico

| Tecnología | Categoría | Estado | Responsable |
|------------|-----------|---------|-------------|
| ASP.NET Core | Framework | Adoptar | |
| ASP Clásico | Framework | Retirar | |
| Web Components | Frontend | Adoptar | |
| RabbitMQ | Integración | Adoptar | |

---

# Justificación

Para cada tecnología documentar.

## Descripción

---

## Casos de Uso

---

## Beneficios

---

## Riesgos

---

## Restricciones

---

## Alternativas

---

## Fecha de Revisión

---

# Relación con Capacidades

Relacionar tecnologías con capacidades.

| Capacidad | Tecnología |
|-----------|------------|
| APIs | ASP.NET Core |
| Integración | RabbitMQ |
| IA | Semantic Kernel |

---

# Relación con ADR

| Tecnología | ADR |
|------------|-----|
| ASP.NET Core | ADR-004 |
| Kubernetes | ADR-015 |

---

# Obsolescencia

Identificar tecnologías próximas al retiro.

| Tecnología | Riesgo | Fecha Objetivo |
|------------|---------|----------------|
| ASP Clásico | Alto | |
| .NET Framework | Medio | |

Definir estrategia de transición.

---

# Innovación

Registrar tecnologías emergentes.

| Tecnología | Estado |
|------------|---------|
| MCP | Evaluar |
| WASM | Probar |
| Platform Engineering | Adoptar |

---

# Riesgos Tecnológicos

| Riesgo | Mitigación |
|---------|------------|
| Vendor Lock-in | |
| Fin de soporte | |
| Escasez de talento | |
| Costos de licencias | |

---

# Roadmap Tecnológico

```text
Evaluar

↓

Probar

↓

Adoptar

↓

Estandarizar

↓

Optimizar

↓

Restringir

↓

Retirar
```

---

# Indicadores

| Indicador | Objetivo |
|------------|-----------|
| Tecnologías Estandarizadas | |
| Tecnologías Obsoletas | |
| Tiempo de Adopción | |
| Cumplimiento del Radar | |

---

# Checklist

## Evaluación

- [ ] Tecnología analizada
- [ ] Riesgos evaluados
- [ ] Alternativas comparadas

---

## Gobernanza

- [ ] ADR relacionado
- [ ] Responsable asignado
- [ ] Fecha de revisión definida

---

## Evolución

- [ ] Roadmap actualizado
- [ ] Obsolescencia identificada
- [ ] Comunicación realizada

---

# Documentos Relacionados

- Enterprise Architecture
- Governance Architecture
- Sustainability Architecture
- Platform Engineering Architecture
- ADR
- Standards

---

# Historial de Versiones

| Versión | Fecha | Descripción |
|----------|------|-------------|
| 1.0 | YYYY-MM-DD | Primera versión |

---

# Aprobaciones

| Rol | Responsable | Fecha |
|------|-------------|------|
| Enterprise Architect | | |
| Architecture Board | | |
| CTO | | |

---

# Declaración Final

El Technology Radar de ARCHE constituye el mecanismo oficial para evaluar, adoptar, estandarizar y retirar tecnologías dentro de la organización.

Su propósito no es recomendar herramientas de forma aislada, sino asegurar que toda decisión tecnológica esté alineada con las capacidades del negocio, los principios arquitectónicos y la estrategia de evolución tecnológica.

El radar debe revisarse periódicamente y entenderse como un instrumento vivo de gobernanza.

---

> **La tecnología envejece.**
>
> **Las decisiones permanecen.**
>
> **El Technology Radar existe para que las decisiones tecnológicas sean conscientes, justificadas y sostenibles.**

---

© Arquetipo Digital
