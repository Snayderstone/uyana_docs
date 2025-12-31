---
sidebar_position: 3
---

# Despliegue

Recomendaciones para entornos de staging y producción.

## Entornos

- **Desarrollo:** ramas feature con despliegue automático a entornos efímeros.
- **Staging:** integración con datos de prueba y smoke tests automáticos.
- **Producción:** despliegue progresivo con canary y rollback automático ante fallos.

## Pipeline sugerido

1. Ejecutar lint, pruebas unitarias y de integración.
2. Construir imágenes y escanear vulnerabilidades.
3. Desplegar a staging y correr smoke tests.
4. Promover a producción con canary y monitoreo activo.

## Configuración

- Variables sensibles gestionadas con un secreto centralizado (ej. Vault/SM).
- Feature flags para activar funcionalidades gradualmente.
- Backups diarios de base de datos y restauración probada mensualmente.
