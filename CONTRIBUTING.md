# Guía de Contribución y Estrategia de Ramificación

Para mantener la calidad del código y la estabilidad en los entornos, este repositorio aplica una estrategia de ramificación basada en ramas por funcionalidad y revisión obligatoria por pares.

## 1. Estructura de Ramas Principales
 `main` Refleja el código estable listo para producción. Protegida contra commits directos.
 `development` Rama principal de integración para el desarrollo actual. Protegida contra commits directos.

## 2. Nomenclatura para Ramas de Trabajo
Ningún desarrollador debe trabajar directamente en `main` o `development`. Todas las tareas se deben realizar en ramas auxiliares creadas a partir de `development`

 `featurenombre-tarea` Para el desarrollo de nuevas historias de usuario o funcionalidades (ej. `featurelogin-jwt`).
 `hotfixnombre-correccion` Para correcciones urgentes de errores detectados (ej. `hotfixfix-cors-error`).

## 3. Flujo de Trabajo (Workflow)
1. Posicionarse en `development` y actualizar
   ```bash
   git checkout development
   git pull origin development