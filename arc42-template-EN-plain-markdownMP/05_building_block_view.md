# Vista de Bloques de Construcción

## Visión general del sistema

El Sistema ERP se ha diseñado con una **arquitectura monolítica simple**, compuesta por tres contenedores principales: una aplicación web (SPA), una API que centraliza la lógica de negocio, y una base de datos relacional.

A continuación se presenta el diagrama de contenedores (Nivel 2 - C2):

![Diagrama de Contenedores](./images/c2_containers.png)

## Descripción de los contenedores

### Single-Page Application (SPA)

- **Tecnología**: JavaScript, React
- **Responsabilidad**: Es la interfaz de usuario que se ejecuta en el navegador del Administrador de Compras. Permite registrar productos, proveedores y crear órdenes de compra. Se comunica con la API mediante peticiones HTTPS/JSON.

### API Monolítica

- **Tecnología**: Java, Spring Boot
- **Responsabilidad**: Maneja toda la lógica de negocio del sistema: validación de datos, reglas del módulo de compras, y comunicación con la base de datos. Expone endpoints REST consumidos por la SPA.

### Base de Datos

- **Tecnología**: PostgreSQL
- **Responsabilidad**: Almacena todos los datos del ERP, incluyendo productos, proveedores, relaciones producto-proveedor y órdenes de compra. La API accede a ella mediante JDBC.
