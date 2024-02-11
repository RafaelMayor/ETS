<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

## Diagrama de casos de uso de una biblioteca:

![](Casos%20de%20uso%20de%20una%20biblioteca.drawio.png)

## Diagrama de secuencia de una biblioteca:

![](DS%20Biblioteca.drawio.png)

# **Casos de Uso de la Biblioteca**

### 1. Prestar Libro
   - **Actor:** Bibliotecario
   - **Descripción:** El bibliotecario presta un libro a un usuario.
   - **Pasos:**
   1. El usuario o el bibliotecario inicia sesión en el sistema de la biblioteca.
   2. El usuario o el bibliotecario busca el libro que desea prestar.
   3. El usuario o el bibliotecario selecciona el libro y lo presta al usuario.

### 2. Devolver Libro
   - **Actor:** Usuario
   - **Descripción:** El usuario devuelve un libro a la biblioteca.
   - **Pasos:**
   1. El usuario inicia sesión en el sistema de la biblioteca.
   2. El usuario selecciona el libro que desea devolver.
   3. El usuario devuelve el libro al bibliotecario.

### 3. Buscar Libro
   - **Actor:** Usuario, Bibliotecario
   - **Descripción:** Se busca un libro específico en la biblioteca.
   - **Pasos:**
   1. El usuario o el bibliotecario inicia sesión en el sistema de la biblioteca.
   2. El usuario o el bibliotecario busca el libro que desea encontrar.

### 4. Alargar Plazo de Entrega
   - **Actor:** Usuario 
   - **Descripción:** El usuario solicita más tiempo para tener prestado un libro.
   - **Pasos:**
   1. El bibliotecario inicia sesión en el sistema de la biblioteca.
   2. El bibliotecario busca el libro que desea extender el plazo de entrega.
   3. El bibliotecario selecciona el libro y extiende el plazo de entrega.

### 5.Donar Libro 
   - **Actor:** Usuario 
   - **Descripción:** Un usuario dona libros a la biblioteca para agregar al inventario existente.
   - **Pasos:**
   1. El usuario inicia sesión en el sistema de la biblioteca.
   2. El usuario selecciona la opción de donar un libro.
   3. El usuario ingresa la información del libro que desea donar y lo dona a la biblioteca.


## **Tabla de descripción de cada actor:**

| Actor | Descripción | Características | Relaciones | Referencias | Autor | Fecha |
|---|---|---|---|---|---|---|
| **Usuario** | Persona que desea utilizar los servicios de la biblioteca. | - Puede ser un estudiante, un trabajador, un jubilado, etc. - Puede ser un lector habitual o esporádico. | **Bibliotecario** | **Devolver libro**, **Buscar libro**, **Donar libro** | Rafael Martín Mayor | 2024-01-28 |
| **Bibliotecario** | Persona responsable de gestionar los recursos de la biblioteca. | - Tiene formación en biblioteconomía. - Tiene experiencia en el manejo de sistemas de información. | **Usuario** | **Prestar libro**, **Buscar libro**, **Alargar plazo de entrega** | Rafael Martín Mayor | 2024-01-28 |


## **Tabla de descripción de cada caso de uso:**


**Caso de Uso** | **Actores** | **Descripción** | **Flujo básico** | **Pre-condiciones** | **Post-condiciones** | **Requerimientos** | **Notas** | **Autor** | **Fecha**
---|---|---|---|---|---|---|---|---|---|
**Prestar libro** | **Bibliotecario** | El usuario solicita un libro de la biblioteca. | 1. El usuario se identifica en el sistema. 2. El usuario selecciona el libro que desea prestar. 3. El bibliotecario verifica la disponibilidad del libro. 4. El bibliotecario presta el libro al usuario. 5. El usuario recibe el libro. | El usuario debe estar registrado en la biblioteca. El libro debe estar disponible en la biblioteca. | El libro se encuentra en el inventario de la biblioteca. El usuario tiene el préstamo del libro. | Tarjeta de identificación de la biblioteca. | El bibliotecario puede rechazar la solicitud de préstamo si el libro no está disponible o si el usuario tiene una deuda pendiente con la biblioteca. | Rafael Martín Mayor | 2024-01-28
**Devolver libro** | **Usuario** | El usuario devuelve un libro a la biblioteca. | 1. El usuario se identifica en el sistema. 2. El usuario presenta el libro que desea devolver. 3. El bibliotecario verifica la condición del libro. 4. El bibliotecario devuelve el libro al inventario. 5. El usuario recibe un recibo de devolución. | El usuario debe estar registrado en la biblioteca. El usuario debe tener el libro que desea devolver. | El libro se encuentra en el inventario de la biblioteca. El usuario no tiene una deuda pendiente con la biblioteca. | Tarjeta de identificación de la biblioteca. | El bibliotecario puede rechazar la devolución del libro si el libro no está en buenas condiciones o si el usuario tiene una deuda pendiente con la biblioteca. | Rafael Martín Mayor | 2024-01-28
**Buscar libro** | **Usuario**, **Bibliotecario** | El usuario/bibliotecario busca un libro en la biblioteca. | 1. El usuario/bibliotecario se identifica en el sistema. 2. El usuario/bibliotecario ingresa los datos del libro que desea buscar. 3. El sistema muestra los resultados de la búsqueda. | El usuario/bibliotecario debe estar registrado en la biblioteca. | El sistema muestra los resultados de la búsqueda que coinciden con los datos ingresados por el usuario/bibliotecario. | N/A | El usuario/bibliotecario puede buscar por título, autor, editorial, tema, etc. | Rafael Martín Mayor | 2024-01-28
**Alargar plazo de entrega** | **Bibliotecario** | El bibliotecario hace una prórroga del plazo de entrega de un libro prestado. | 1. El usuario se identifica en el sistema. 2. El usuario selecciona el libro que desea prorrogar. 3. El bibliotecario verifica la disponibilidad del libro. 4. El bibliotecario autoriza la prórroga. 5. El sistema actualiza la fecha de devolución del libro. | El usuario debe estar registrado en la biblioteca. El libro debe estar disponible en la biblioteca. El usuario debe tener una deuda pendiente con la biblioteca. | El plazo de entrega del libro se prorroga. | Tarjeta de identificación de la biblioteca. | El bibliotecario puede rechazar la solicitud de prórroga si el libro no está disponible o si el usuario tiene una deuda pendiente con la biblioteca. | Rafael Martín Mayor | 2024-01-28
**Donar libro** | **Usuario** | El usuario dona un libro a la biblioteca. | 1. El usuario se identifica en el sistema. 2. El usuario presenta el libro que desea donar. 3. El bibliotecario verifica la condición del libro. 4. El bibliotecario registra la donación. 5. El usuario recibe un certificado de donación. | El usuario debe estar registrado en la biblioteca. El libro debe estar en buenas condiciones. | El libro se agrega al inventario de la biblioteca. El usuario recibe un certificado de donación. | N/A | El bibliotecario puede rechazar la donación si el libro no está en buenas condiciones. | Rafael Martín Mayor | 2024-01-28


## **Tabla de especificación de casos de uso:**


| Caso de uso | Precondición | Descripción | Secuencia normal | Postcondición | Excepciones |
|---|---|---|---|---|---|
| **Prestar libro** | El usuario está registrado en la biblioteca y tiene una cuenta activa. | El usuario solicita un libro a la biblioteca para su préstamo. | 1. El usuario se identifica en el sistema de la biblioteca. 2. El usuario selecciona el libro que desea prestar. 3. El sistema verifica la disponibilidad del libro. 4. El sistema registra el préstamo del libro. 5. El sistema entrega el libro al usuario. | El libro está prestado al usuario y el usuario puede leerlo. | Libro no disponible: El sistema informa al usuario de que el libro no está disponible y el caso de uso termina. Usuario no registrado: El sistema informa al usuario de que debe registrarse antes de poder prestar un libro y el caso de uso termina. |
| **Devolver libro** | El usuario tiene un libro prestado de la biblioteca. | El usuario devuelve un libro prestado a la biblioteca. | 1. El usuario se identifica en el sistema de la biblioteca. 2. El usuario presenta el libro que desea devolver. 3. El sistema verifica que el libro sea el correcto. 4. El sistema registra la devolución del libro. 5. El sistema informa al usuario de que la devolución ha sido realizada correctamente. | El libro ha sido devuelto a la biblioteca y está disponible para ser prestado de nuevo. | Libro no reconocido: El sistema informa al usuario de que el libro no está registrado en el sistema y el caso de uso termina. |
| **Buscar libro** | El usuario tiene acceso al sistema de la biblioteca. | El usuario busca un libro en la biblioteca. | 1. El usuario introduce los datos del libro que desea buscar. 2. El sistema busca el libro en la base de datos. 3. El sistema muestra los resultados de la búsqueda al usuario. | El usuario tiene acceso a la información sobre el libro que buscaba. | Libro no encontrado: El sistema informa al usuario de que el libro no se encuentra en la base de datos y el caso de uso termina. |
| **Alargar plazo de entrega** | El usuario tiene un libro prestado de la biblioteca. | El usuario solicita a la biblioteca alargar el plazo de entrega de un libro prestado. | 1. El usuario se identifica en el sistema de la biblioteca. 2. El usuario solicita alargar el plazo de entrega de un libro prestado. 3. El sistema verifica que el usuario tiene derecho a alargar el plazo de entrega. 4. El sistema extiende el plazo de entrega del libro. 5. El sistema informa al usuario de que el plazo de entrega ha sido extendido. | El plazo de entrega del libro ha sido extendido. | Usuario no autorizado: El sistema informa al usuario de que no tiene derecho a alargar el plazo de entrega y el caso de uso termina. Plazo máximo de entrega superado: El sistema informa al usuario de que el plazo máximo de entrega ya ha sido superado y el caso de uso termina. |
| **Donar libro** | El usuario tiene un libro que desea donar a la biblioteca. | El usuario dona un libro a la biblioteca. | 1. El usuario se identifica en el sistema de la biblioteca. 2. El usuario presenta el libro que desea donar. 3. El sistema verifica que el libro es apto para ser donado. 4. El sistema registra la donación del libro. 5. El sistema informa al usuario de que la donación ha sido aceptada. | El libro ha sido donado a la biblioteca y está disponible para otros usuarios. | Libro no apto para ser donado: El sistema informa al usuario de que el libro no es apto para ser donado y el caso de uso termina. |


</div>