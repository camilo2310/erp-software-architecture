# Vista de Tiempo de Ejecución

## Escenario: Registrar un Producto

Este escenario describe el flujo de interacción entre los contenedores del sistema cuando el Administrador de Compras registra un nuevo producto, correspondiente a la historia de usuario: *"Como gestor de inventario, quiero registrar nuevos productos con su información básica, para que pueda mantener un catálogo actualizado para las compras."*

![Diagrama de Secuencia](./images/sequence_registrar_producto.png)

## Descripción del flujo

1. El **Administrador** rellena el formulario de nuevo producto en la **SPA** y lo envía.
2. La **SPA** realiza una petición `POST /api/productos` hacia la **API**, enviando los datos capturados.
3. La **API** valida los datos recibidos (por ejemplo, que el campo "nombre" no esté vacío).
4. Si la validación es exitosa, la **API** ejecuta una instrucción `INSERT INTO productos` sobre la **Base de Datos**.
5. La **Base de Datos** confirma la creación del registro y devuelve el producto con su ID generado.
6. La **API** responde a la **SPA** con un código `201 Created` y los datos del producto creado.
7. La **SPA** muestra un mensaje de éxito al Administrador y actualiza la lista de productos en pantalla.

Este flujo garantiza que solo se registren productos con información válida, cumpliendo los criterios de aceptación definidos en el backlog.
