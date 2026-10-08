- Mi Perfil en GitHub Pages — IF-1116

Sitio web personal desarrollado para la asignatura IF-1116 (Semestre 2026-II).

- Demo
Puedes ver la página publicada en: [https://GuillermoVelarde.github.io](https://GuillermoVelarde.github.io)

- Tecnologías Utilizadas
HTML5
CSS3
Git & GitHub

 - Flujo de Trabajo Demostrado
Commits atómicos**: Registros estructurados por cada sección agregada.
Flujo basado en ramas**: Trabajo colaborativo con ramas `feature/*` y `fix/*`.
Pull Requests & Merge**: Integración continua a la rama `main`.
Resolución de conflictos**: Manejo y resolución de conflictos de código localmente.

## Delivery o Deployment

Este proyecto implementa un esquema de **Continuous Delivery** debido a que, aunque todas las fases de integración (compilación, pruebas unitarias con Vitest, construcción de imagen Docker, escaneo de seguridad con Trivy y pruebas smoke) se ejecutan de forma automatizada, la publicación final a producción (`deploy-prod`) requiere una **aprobación manual** mediante las reglas de protección del entorno `github-pages`.

Para convertir este flujo a **Continuous Deployment**, bastaría con remover la regla de revisión obligatoria (*required reviewers*) en la configuración del entorno `github-pages` en GitHub, logrando que el despliegue se ejecute automáticamente tras superar la etapa de `smoke`.
