---
title: <Arquitectura de Seguridad>
id: ARC-SEC-180
version: 1.0
status: Draft
owner: Arquetipo Digital
category: Architecture
type: Security Architecture
domain: Security
framework: ARCHE
classification: Cross-Cutting
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
  - ARC-CLD-130 Cloud Architecture
  - ARC-DAT-150 Data Architecture
  - ADS-003 Quality Attribute Scenarios
  - ADS-004 Architecture Decision Standard
tags:
  - architecture
  - security
---

# Arquitectura de Seguridad

> La seguridad no consiste en agregar controles al final del proyecto.
>
> Consiste en diseñar una arquitectura donde proteger los activos sea una propiedad natural del sistema.

---

# Resumen Ejecutivo

Describir:

- activos protegidos;
- principales riesgos;
- estrategia de seguridad;
- controles implementados;
- beneficios esperados.

---

# Información General

| Campo | Valor |
|--------|-------|
| Proyecto | |
| Organización | |
| Arquitecto de Seguridad | |
| Estado | |
| Versión | |

---

# Contexto

## Problema

¿Qué riesgos justifican esta arquitectura?

---

## Objetivos

### Negocio

-

### Seguridad

-

### Cumplimiento

-

---

# Activos del Negocio

Identificar los activos críticos.

| Activo | Criticidad |
|---------|------------|
| Información de clientes | Alta |
| Consentimientos | Alta |
| Credenciales | Alta |
| Datos financieros | Alta |

---

# Clasificación de la Información

| Tipo | Ejemplo |
|------|----------|
| Pública | |
| Uso Interno | |
| Confidencial | |
| Restringida | |

---

# Evaluación de Riesgos

| Riesgo | Probabilidad | Impacto | Nivel |
|---------|--------------|---------|-------|
| Riesgo | | | |

Documentar metodología utilizada.

---

# Modelo de Amenazas

Identificar amenazas.

Ejemplos.

- Acceso no autorizado
- Robo de credenciales
- Fuga de información
- Ataques internos
- Denegación de Servicio
- Supply Chain
- Prompt Injection (IA)

Cuando sea posible utilizar STRIDE, ATT&CK u otra metodología reconocida.

---

# Principios de Seguridad

Aplicar.

- Security by Design
- Zero Trust
- Least Privilege
- Defense in Depth
- Secure by Default
- Fail Secure
- Segregación de funciones

Justificar su aplicación.

---

# Arquitectura General

Agregar diagrama.

```text
Usuario

↓

Identidad

↓

Canal Seguro

↓

Aplicación

↓

Servicios

↓

Datos

↓

Auditoría
```

---

# Identidad y Acceso

## Autenticación

Documentar.

- OAuth2
- OIDC
- SAML
- MFA
- Passkeys
- Certificados

---

## Autorización

Describir.

- Roles
- Claims
- Policies
- Scopes
- ABAC
- RBAC

---

## Gestión de Identidades

Documentar.

- IAM
- Directorios
- Federaciones
- Ciclo de vida de usuarios

---

# Protección de Datos

Documentar.

## En tránsito

- TLS
- mTLS

---

## En reposo

- Cifrado
- KMS
- HSM

---

## Datos sensibles

- Enmascaramiento
- Tokenización
- Anonimización

---

# Seguridad de Aplicaciones

Documentar.

- Validaciones
- Sanitización
- Gestión de sesiones
- Protección CSRF
- Protección XSS
- Protección SSRF
- Protección SQL Injection

---

# Seguridad de APIs

Documentar.

- API Gateway
- Rate Limit
- Throttling
- API Keys
- OAuth
- mTLS
- JWT

---

# Seguridad Cloud

Documentar.

- IAM
- Key Vault
- Security Groups
- WAF
- Bastion
- Redes privadas

---

# Seguridad de Integraciones

Documentar.

- firma digital;
- cifrado;
- autenticación mutua;
- validación de mensajes;
- replay protection.

---

# DevSecOps

Documentar.

- SAST
- DAST
- SCA
- Secret Scanning
- SBOM
- IaC Scanning
- Container Scanning

---

# Observabilidad de Seguridad

Documentar.

- auditoría;
- SIEM;
- correlación;
- alertas;
- detección;
- respuesta.

Herramientas.

- Microsoft Sentinel
- Splunk
- Elastic
- QRadar

---

# Cumplimiento

Indicar normas aplicables.

- ISO 27001
- NIST CSF
- CIS Controls
- OWASP ASVS
- PCI DSS
- GDPR
- Ley Marco de Ciberseguridad (Chile)
- Otras regulaciones aplicables

---

# Respuesta ante Incidentes

Definir.

- detección;
- contención;
- erradicación;
- recuperación;
- lecciones aprendidas.

---

# Atributos de Calidad

| Atributo | Estrategia |
|----------|------------|
| Confidencialidad | |
| Integridad | |
| Disponibilidad | |
| Trazabilidad | |
| No Repudio | |

---

# Riesgos Residuales

Documentar.

| Riesgo | Mitigación | Riesgo Residual |
|---------|------------|-----------------|
| Riesgo | | |

---

# ADR Relacionados

Referenciar decisiones de seguridad.

---

# Checklist

## Diseño

- [ ] Activos identificados
- [ ] Riesgos evaluados
- [ ] Amenazas modeladas

---

## Controles

- [ ] IAM definido
- [ ] Cifrado implementado
- [ ] Auditoría habilitada

---

## DevSecOps

- [ ] SAST
- [ ] DAST
- [ ] SCA
- [ ] SBOM

---

## Gobernanza

- [ ] ADR registrados
- [ ] Revisión realizada
- [ ] Cumplimiento validado

---

# Documentos Relacionados

- Enterprise Architecture
- Solution Architecture
- Software Architecture
- Cloud Architecture
- Data Architecture
- AI Architecture
- Integration Architecture
- Deployment Architecture
- ADR

---

# Historial de Versiones

| Versión | Fecha | Descripción |
|----------|------|-------------|
| 1.0 | YYYY-MM-DD | Primera versión |

---

# Aprobaciones

| Rol | Responsable | Fecha |
|------|-------------|------|
| Security Architect | | |
| CISO | | |
| Enterprise Architect | | |

---

# Declaración Final

La Arquitectura de Seguridad define cómo una organización protege sus activos críticos mediante principios, controles y decisiones arquitectónicas alineadas con el riesgo y los objetivos del negocio.

Su propósito no es incorporar herramientas de seguridad, sino construir soluciones resilientes, verificables y preparadas para evolucionar frente a nuevas amenazas.

---

> **No protegemos servidores.**
>
> **No protegemos aplicaciones.**
>
> **Protegemos el valor que representan para el negocio.**
>
> **La tecnología es solo uno de los mecanismos para lograrlo.**

---

© Arquetipo Digital
