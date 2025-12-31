---
sidebar_position: 1
---

# Arquitectura

Panorama general de la plataforma Uyana para equipos técnicos.

## Componentes principales

- **Front-end:** React + Docusaurus para la documentación y React SPA para la aplicación principal.
- **API:** Servicios REST/GraphQL detrás de un gateway con autenticación basada en tokens.
- **Datos:** Base de datos relacional para la capa transaccional y almacén analítico para reportes.
- **Mensajería:** Cola de eventos para orquestar tareas asíncronas y notificaciones.

## Seguridad

- Autenticación mediante SSO o credenciales internas con MFA opcional.
- Autorización basada en roles y permisos por recurso.
- Cifrado en tránsito (HTTPS) y en reposo para datos sensibles.

## Observabilidad

- Métricas y trazas expuestas a través de un stack de observabilidad centralizado.
- Alertas configuradas para errores 5xx, latencias elevadas y fallos de jobs programados.
