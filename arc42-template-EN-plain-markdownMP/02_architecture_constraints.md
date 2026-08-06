# Restricciones de Arquitectura

## Decisiones tecnológicas

Para el desarrollo del Sistema ERP se han tomado las siguientes decisiones tecnológicas:

- **Backend**: Se usará Java con el framework Spring Boot para exponer una API REST que maneje toda la lógica de negocio.
- **Frontend**: La interfaz de usuario será una Single-Page Application (SPA) construida con JavaScript y React.
- **Base de datos**: Se usará PostgreSQL como sistema de gestión de base de datos relacional.
- **Comunicación**: El frontend y el backend se comunicarán mediante peticiones HTTPS con formato JSON.

## Restricciones organizacionales

- El proyecto debe seguir una metodología ágil (Scrum/Kanban), gestionando el trabajo mediante un backlog priorizado.
- La documentación de arquitectura debe mantenerse actualizada en el repositorio de código bajo la plantilla arc42.
- El control de versiones se realizará mediante Git, con el repositorio alojado en GitHub.

## Convenciones

- Los diagramas de arquitectura se modelan utilizando el estándar C4 (Contexto y Contenedores) con notación PlantUML.
- El diseño detallado de componentes se documenta mediante diagramas UML (secuencia y entidad-relación).
