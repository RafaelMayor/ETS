<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

## Diagrama de casos de uso de Sistema de Gestión de Tienda en Línea:

![](Sistema%20de%20Gestión%20de%20Tienda%20en%20Línea.drawio.png)

## Diagrama de secuencia de Sistema de Gestión de Tienda en Línea:

![](DS%20Sistema%20de%20Gestión%20de%20Tienda%20en%20Línea.drawio.png)

## Diagrama de actividades de Sistema de Gestión de Tienda en Línea:

![](DAct%20Sistema%20de%20Gestión%20de%20Tienda%20en%20Línea.png)

## Diagrama de clases de Sistema de Gestión de Tienda en Línea:

![](DC%20Sistema%20de%20Gestión%20de%20Tienda%20en%20Línea.png)

## Diagrama de objetos de Sistema de Gestión de Tienda en Línea:

![](DObj%20Sistema%20de%20Gestión%20de%20Tienda%20en%20Línea.png)


# Sistema de Gestión de Tienda en Línea

1. **Gestionar Inventario (Administrador):**
   - El administrador revisa y actualiza el inventario existente.
   - Pasos:
     1. El administrador inicia sesión en el sistema.
     2. Selecciona la opción para gestionar inventario.
     3. Revisa los productos existentes, sus cantidades y detalles.
     4. Actualiza la información según sea necesario.

2. **Editar Catálogo (Administrador):**
   - El administrador añade, elimina o modifica productos en el catálogo online.
   - Pasos:
     1. El administrador inicia sesión en el sistema.
     2. Selecciona la opción para editar catálogo.
     3. Añade, elimina o modifica información del producto según sea necesario.

3. **Ver Catálogo (Cliente):**
   - Los clientes pueden ver los productos disponibles en línea.
   - Pasos:
     1. El usuario abre la tienda en línea.
     2. Navega a través del catálogo de productos disponibles.

4. **Realizar Compra (Cliente):**
   - Los clientes seleccionan productos y completan la compra online.
   - Pasos:
     1. El cliente selecciona productos del catálogo.
     2. Añade los productos al carrito de compras.
     3. Procede al pago y completa la compra.

5. **Realizar reembolso (Cliente/Administrador):**
   - El administrador procesa solicitudes de reembolso por parte de los clientes.
   - Pasos:
     1. El cliente solicita un reembolso a través del sistema online o contacto directo.
     2. El administrador revisa la solicitud.
     3. Se procesa el reembolso si es aplicable.


## **Tabla de descripción de cada actor:**

| Actor | Descripción | Características | Relaciones | Referencias | Autor | Fecha |
|---|---|---|---|---|---|---|
| **Cliente** | Persona que realiza compras en la tienda en línea. | - Usuario final del sistema. - Puede ser un consumidor individual o una empresa. | Administrador | **Ver catálogo**, **Realizar compra**, **Realizar reembolso** | Rafael Martín Mayor | 2024-01-28 |
| **Administrador** | Persona que gestiona la tienda en línea. | - Usuario autorizado del sistema. - Tiene conocimientos técnicos sobre el funcionamiento del sistema. | Cliente | **Gestionar inventario**, **Editar catálogo**, **Realizar reembolso** | Rafael Martín Mayor | 2024-01-28 |

## **Tabla de especificación de casos de uso:**

| Caso de Uso | Actores | Descripción | Precondición | Secuencia normal | Postcondición | Excepciones | Autor | Fecha |
|---|---|---|---|---|---|---|---|---|
| **Ver catálogo** | Cliente | El cliente puede ver el catálogo de productos de la tienda. | El cliente debe estar registrado o ser un invitado. | El cliente inicia sesión o crea una cuenta de invitado. El cliente selecciona un producto del catálogo. El sistema muestra la información del producto. El cliente puede navegar por el catálogo y seleccionar otros productos. | El cliente tiene una lista de los productos que ha seleccionado. | El producto no está disponible. El sistema muestra un mensaje de error al cliente y le permite seleccionar otro producto. El cliente no está registrado o no ha iniciado sesión. El sistema muestra un mensaje de error al cliente y le permite registrarse o iniciar sesión. | Rafael Martín Mayor | 2024-01-28 |
| **Realizar compra** | Cliente | El cliente puede realizar una compra de los productos seleccionados. | El cliente debe tener una lista de productos seleccionados. | El cliente inicia sesión o crea una cuenta de invitado. El cliente selecciona un método de pago. El cliente introduce los datos de pago. El sistema confirma la compra. | El sistema envía un correo electrónico de confirmación al cliente. | El cliente no tiene una lista de productos seleccionados. El método de pago no es válido. El sistema muestra un mensaje de error al cliente y le permite seleccionar otro método de pago. | Rafael Martín Mayor | 2024-01-28 |
| **Gestionar inventario** | Administrador | El administrador puede gestionar el inventario de la tienda. | El administrador debe usar su cuenta de administrador. | El administrador inicia sesión. El administrador selecciona una acción de inventario. El administrador introduce los datos necesarios. El sistema realiza la acción. | El inventario se actualiza. | El administrador no está autorizado, ha iniciado sesión con una cuenta cliente, debe iniciar sesión con una cuenta de administrador. El dato introducido no es válido. El sistema muestra un mensaje de error al administrador y le permite introducir los datos nuevamente. | Rafael Martín Mayor | 2024-01-28 |
| **Editar catálogo** | Administrador | El administrador puede editar el catálogo de productos de la tienda. | El administrador debe usar su cuenta de administrador. | El administrador inicia sesión. El administrador selecciona un producto del catálogo. El administrador edita la información del producto. El sistema guarda los cambios. | La información del producto se actualiza. | El producto no existe. El sistema muestra un mensaje de error al administrador y le permite seleccionar otro producto. El dato introducido no es válido. El sistema muestra un mensaje de error al administrador y le permite introducir los datos nuevamente. | Rafael Martín Mayor | 2024-01-28 |
| **Realizar reembolso** | Administrador, Cliente | El administrador puede realizar un reembolso a un cliente. | El reembolso pude ser efectuado si la compra no se hizo hace más de 30 días | El administrador inicia sesión. El administrador selecciona una compra. El administrador introduce el monto del reembolso. El sistema realiza el reembolso. | El cliente recibe un correo electrónico de confirmación del reembolso. | El cliente no tiene una compra. El sistema muestra un mensaje de error al administrador y le invita a seleccionar un producto. El monto del reembolso no es válido. O bien el cliente no ha introducido bien el monto o el cliente realizó la compra hace más de 30 días y no puede reembolsar. | Rafael Martín Mayor | 2024-01-28 |

</div>