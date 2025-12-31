---
sidebar_position: 2
---

# Integraciones

Lineamientos para conectar Uyana con servicios externos.

## Webhooks

- Registra webhooks desde **Ajustes > Integraciones**.
- Eventos disponibles: creación/actualización de tareas, cambios de estado, comentarios y adjuntos.
- Firma HMAC incluida en el header `X-Uyana-Signature`; verifica antes de procesar.

## API

- Autenticación con tokens de servicio (Bearer).
- Rate limit estándar: 500 solicitudes/minuto por token.
- Usa cabeceras `Idempotency-Key` para operaciones que crean recursos.
- Consulta la referencia de endpoints en `https://api.uyana.com/docs` (placeholder).

## Single Sign-On

- Soporte para SAML 2.0 y OpenID Connect.
- Proporciona metadata del IdP y URL de ACS para completar el alta.
- Mapea grupos del IdP a roles internos (admin, colaborador, lector).
