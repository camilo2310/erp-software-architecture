# Alcance y Contexto del Sistema

## Contexto de negocio

El Sistema ERP interactúa principalmente con el **Administrador de Compras**, quien utiliza la plataforma para registrar productos y proveedores, y con un **Sistema Contable Externo**, al cual se le envían los datos de facturas y asientos contables generados por las operaciones del ERP.

A continuación se presenta el diagrama de contexto (Nivel 1 - C1), que muestra el sistema como una caja negra y sus interacciones con actores y sistemas externos:

![Diagrama de Contexto](./images/c1_context.png)

## Descripción de las interacciones

| Actor / Sistema | Interacción |
|---|---|
| Administrador de Compras | Registra productos y proveedores en el sistema ERP |
| Sistema Contable Externo | Recibe datos de facturas y asientos contables enviados por el ERP |

## Contexto técnico

La comunicación entre el Administrador de Compras y el Sistema ERP se realiza a través de un navegador web mediante el protocolo HTTPS. La integración con el Sistema Contable Externo se realizará mediante el envío periódico de datos contables (a definir el mecanismo exacto en una fase posterior del proyecto).
