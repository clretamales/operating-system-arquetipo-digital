---
title: Playbook de Revisión de Seguridad
id: PB-080
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
  - ARC-SEC-180 Security Architecture
  - ARC-RES-220 Resilience Architecture
  - ARC-GOV-200 Governance Architecture
  - ARC-QA-210 Quality Attributes
  - ADS-004 Architecture Decision Standard
tags:
  - security
  - review
  - secure-by-design
---

# Playbook de Revisión de Seguridad

> La seguridad no es una auditoría al final del proyecto.
>
> Es un criterio arquitectónico que debe acompañar todo el ciclo de vida de la solución.

---

# Propósito

Este playbook define el proceso oficial para revisar la seguridad de una solución dentro del framework ARCHE.

Su objetivo es garantizar que los riesgos sean identificados, evaluados y tratados antes de convertirse en vulnerabilidades operacionales.

---

# Principios

Toda revisión de seguridad debe cumplir los siguientes principios.

- Security by Design.
- Riesgo antes que tecnología.
- Zero Trust como principio arquitectónico.
- Menor privilegio.
- Defensa en profundidad.
- Automatización siempre que sea posible.
- Evidencia antes que percepción.

---

# Flujo General

```text
Activos

↓

Amenazas

↓

Riesgos

↓

Controles

↓

Arquitectura

↓

Validación

↓

Operación

↓

Revisión Continua
```

---

# Paso 1. Identificar Activos

Responder.

- ¿Qué protege la solución?
- ¿Qué información es crítica?
- ¿Qué procesos son esenciales?
- ¿Qué servicios no pueden fallar?

Clasificar activos.

| Activo | Criticidad |
|---------|------------|
| Datos personales | Alta |
| Credenciales | Alta |
| Consentimientos | Alta |
| Información pública | Baja |

---

# Paso 2. Clasificar la Información

Definir.

- Pública.
- Uso Interno.
- Confidencial.
- Restringida.

Relacionar con Data Architecture.

---

# Paso 3. Identificar Amenazas

Aplicar metodologías cuando corresponda.

Ejemplos.

- STRIDE
- MITRE ATT&CK
- OWASP Top 10
- OWASP API Top 10

Documentar.

- amenaza;
- origen;
- impacto.

---

# Paso 4. Evaluar Riesgos

Para cada riesgo registrar.

- probabilidad;
- impacto;
- criticidad;
- mitigación.

Utilizar una matriz de riesgos.

---

# Paso 5. Revisar la Arquitectura

Verificar.

## Identidad

- IAM
- MFA
- Federaciones

---

## Autorización

- RBAC
- ABAC
- Policies

---

## Datos

- cifrado;
- tokenización;
- enmascaramiento.

---

## Integraciones

- OAuth2
- OIDC
- mTLS
- JWT

---

## Infraestructura

- segmentación;
- WAF;
- firewalls;
- redes privadas.

---

# Paso 6. Validar Controles

Revisar.

- autenticación;
- autorización;
- validación de entradas;
- gestión de sesiones;
- protección CSRF;
- protección XSS;
- protección SSRF;
- protección SQL Injection.

---

# Paso 7. Validar DevSecOps

Verificar.

- SAST.
- DAST.
- SCA.
- Secret Scanning.
- Container Scanning.
- IaC Scanning.
- SBOM.

---

# Paso 8. Revisar Observabilidad

Comprobar.

- auditoría;
- logs;
- alertas;
- correlación;
- trazabilidad.

Toda acción relevante debe ser trazable.

---

# Paso 9. Validar Resiliencia

Revisar.

- backups;
- recuperación;
- RTO;
- RPO;
- continuidad.

Relacionar con Resilience Architecture.

---

# Paso 10. Revisar Cumplimiento

Evaluar cumplimiento con.

- ISO 27001.
- NIST CSF.
- CIS Controls.
- OWASP ASVS.
- PCI DSS.
- GDPR.
- Ley Marco de Ciberseguridad (Chile), cuando aplique.
- Otras normativas aplicables.

---

# Paso 11. Revisar ADR

Verificar.

- decisiones de seguridad;
- excepciones;
- riesgos aceptados.

Toda excepción debe estar documentada.

---

# Paso 12. Elaborar Informe

El informe debe incluir.

- hallazgos;
- riesgos;
- recomendaciones;
- prioridad;
- responsables;
- fecha objetivo.

---

# Artefactos Esperados

| Artefacto | Obligatorio |
|-----------|-------------|
| Security Architecture | ✓ |
| Threat Model | ✓ |
| Risk Assessment | ✓ |
| ADR | ✓ |
| Security Review Report | ✓ |

---

# Checklist

## Activos

- [ ] Activos identificados.
- [ ] Clasificación realizada.
- [ ] Responsables definidos.

---

## Arquitectura

- [ ] IAM validado.
- [ ] Integraciones revisadas.
- [ ] Datos protegidos.

---

## Desarrollo

- [ ] SAST ejecutado.
- [ ] DAST ejecutado.
- [ ] Dependencias revisadas.
- [ ] Secretos protegidos.

---

## Operación

- [ ] Logs auditables.
- [ ] Alertas configuradas.
- [ ] Respuesta ante incidentes documentada.

---

## Gobernanza

- [ ] ADR registrados.
- [ ] Riesgos aceptados formalmente.
- [ ] Architecture Review realizada.

---

# Antipatrones

Evitar.

- Revisar la seguridad únicamente antes de producción.
- Confiar exclusivamente en herramientas automáticas.
- Compartir credenciales.
- Mantener privilegios permanentes sin justificación.
- Exponer servicios sin autenticación.
- Almacenar secretos en código fuente.
- Registrar información sensible en logs.
- Tratar la seguridad como responsabilidad exclusiva del equipo de ciberseguridad.

---

# Indicadores

| Indicador | Objetivo |
|-----------|----------|
| Vulnerabilidades críticas abiertas | |
| Tiempo medio de corrección | |
| Cobertura SAST | |
| Cobertura DAST | |
| Hallazgos repetitivos | |
| Excepciones vigentes | |
| Cumplimiento de estándares | |

---

# Roles

| Rol | Responsabilidad |
|------|-----------------|
| Security Architect | Revisión arquitectónica |
| Enterprise Architect | Alineación estratégica |
| Solution Architect | Diseño seguro |
| Software Architect | Controles de aplicación |
| DevSecOps Engineer | Automatización |
| CISO | Aceptación de riesgos |
| Product Owner | Priorización del riesgo de negocio |

---

# Relación con ARCHE

```text
Enterprise Architecture
        │
        ▼
Security Architecture
        │
        ▼
Threat Modeling
        │
        ▼
Risk Assessment
        │
        ▼
Architecture Review
        │
        ▼
DevSecOps
        │
        ▼
Producción
        │
        ▼
Observabilidad
        │
        ▼
Revisión Continua
```

---

# Criterios de Éxito

Una revisión de seguridad cumple con ARCHE cuando:

- Los activos críticos están identificados y clasificados.
- Las amenazas y riesgos han sido evaluados de forma explícita.
- Los controles están alineados con el nivel de riesgo.
- La arquitectura incorpora seguridad desde el diseño.
- Las decisiones relevantes están respaldadas por ADR.
- Existen evidencias objetivas de validación técnica y operativa.
- La revisión genera acciones concretas y medibles.

---

# Declaración Final

La revisión de seguridad en ARCHE constituye un proceso continuo de evaluación y mejora que busca proteger los activos de mayor valor para el negocio.

Su propósito no es encontrar errores al final del desarrollo, sino fortalecer la arquitectura mediante decisiones fundamentadas, controles proporcionales al riesgo y mecanismos permanentes de verificación.

La seguridad es una capacidad transversal que acompaña todo el ciclo de vida de la solución.

---

> **La mejor vulnerabilidad es la que nunca llega a producción.**
>
> **La mejor revisión de seguridad es la que ocurre antes de escribir el código.**
>
> **La seguridad no retrasa los proyectos; evita que los proyectos fracasen.**

---

© Arquetipo Digital
