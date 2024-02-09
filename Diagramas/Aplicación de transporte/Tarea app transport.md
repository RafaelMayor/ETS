<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

# Tarea app transport

Según la descripción de la imagen, el diagrama de casos de uso representa una aplicación relacionada con el transporte. Hay tres actores involucrados: Administrador, Usuario y sistema ext posic. El Administrador tiene casos de uso como definir los medios de transporte, definir el precio del transporte, agregar o eliminar usuarios y verificar credenciales. El Usuario está asociado con el inicio de sesión, geoposicionamiento, definición de destino, modificación de ruta y sugerencia de destinos interesantes. El actor del sistema de posicionamiento externo está conectado con la visualización de puntos de interés en la ruta. Las flechas indican las interacciones entre los actores y los casos de uso.

A continuación, se presenta una especificación de los casos de uso asociados al diagrama:

## **Casos de uso**

### **Administrador**

    1. Definir medio de transporte: El Administrador puede definir los medios de transporte disponibles en la aplicación. Para ello, debe ingresar la información del medio de transporte, como el nombre, la capacidad, la velocidad y la disponibilidad.

    2. Definir precio del transporte: El Administrador puede definir el precio del transporte para cada medio de transporte disponible en la aplicación. Para ello, debe ingresar la información del precio, como el costo por kilómetro, el costo por minuto y el costo base.

    3. Agregar o eliminar usuarios: El Administrador puede agregar o eliminar usuarios de la aplicación. Para ello, debe ingresar la información del usuario, como el nombre, la dirección de correo electrónico y la contraseña.

    4. Verificar credenciales: El Administrador puede verificar las credenciales de los usuarios de la aplicación. Para ello, debe ingresar la información de inicio de sesión del usuario, como la dirección de correo electrónico y la contraseña.


### **Usuario**


    1. Iniciar sesión: El Usuario puede iniciar sesión en la aplicación. Para ello, debe ingresar la información de inicio de sesión, como la dirección de correo electrónico y la contraseña.

    2. Geoposicionamiento: El Usuario puede utilizar la función de geoposicionamiento de la aplicación para determinar su ubicación actual.

    3. Definir destino: El Usuario puede definir el destino al que desea llegar utilizando la aplicación. Para ello, debe ingresar la información del destino, como la dirección o el nombre del lugar.

    4. Modificar ruta: El Usuario puede modificar la ruta que la aplicación ha sugerido para llegar al destino. Para ello, debe ingresar la información de la ruta modificada, como la dirección o el nombre del lugar.

    5. Sugerir destinos interesantes: El Usuario puede sugerir destinos interesantes a otros usuarios de la aplicación. Para ello, debe ingresar la información del destino, como la dirección o el nombre del lugar.

### **Sistema ext posic**

    1. Mostrar puntos de interés en la ruta: El sistema externo de geoposicionamiento puede mostrar puntos de interés en la ruta sugerida por la aplicación.

## **Tabla de descripción de cada actor**

| Actor | Descripción | Características | Relaciones | Referencias | Notas | Autor | Fecha |
|---|---|---|---|---|---|---|---|
| **Administrador** | Persona encargada de gestionar la aplicación. | - Tiene conocimientos de informática. - Tiene acceso a la base de datos. - Puede realizar tareas administrativas como crear, modificar o eliminar usuarios. | - **Usuario** (extend) | - Casos de uso: Alta y baja de usuarios, Definir medio de transporte, Definir precio transporte | - Notas: El administrador tiene acceso a todas las funcionalidades de la aplicación. | **Rafael Martín Mayor** | **2024-01-28** |
| **Usuario** | Persona que utiliza la aplicación para planificar sus viajes. | - Tiene conocimientos básicos de informática. - Puede utilizar un dispositivo móvil o un ordenador. - Puede realizar tareas como definir el destino, modificar la ruta o visualizar los puntos de interés en ruta. | - **Administrador** (extend) | - Casos de uso: Definir destino, Modificar ruta, Mostrar puntos de interés en ruta | - Notas: El usuario puede realizar tareas básicas para planificar sus viajes. | **Rafael Martín Mayor** | **2024-01-28** |
| **Sistema ext posic** | Sistema geoposicinamiento | Localiza al usuario | - **Usuario** (extend) | - Casos de uso: Geoposicionamiento | | **Rafael Martín Mayor** | **2024-01-28** |


Esta tabla describe los dos actores principales de la aplicación **Transporter App**. Cada actor tiene una descripción, características, relaciones, referencias, notas y autor.

**Descripción**

La descripción es una breve descripción del actor. En este caso, la descripción del administrador es "Persona encargada de gestionar la aplicación" y la descripción del usuario es "Persona que utiliza la aplicación para planificar sus viajes".

**Características**

Las características son atributos que describen al actor. En este caso, las características del administrador son "Tiene conocimientos de informática", "Tiene acceso a la base de datos" y "Puede realizar tareas administrativas como crear, modificar o eliminar usuarios". Las características del usuario son "Tiene conocimientos básicos de informática", "Puede utilizar un dispositivo móvil o un ordenador" y "Puede realizar tareas como definir el destino, modificar la ruta o visualizar los puntos de interés en ruta".

**Relaciones**

Las relaciones son las conexiones que tiene un actor con otros actores. En este caso, el administrador tiene una relación con el usuario, ya que ambos realizan tareas relacionadas con la gestión de la aplicación. El administrador extiende al usuario, lo que significa que el administrador puede realizar todas las tareas que puede realizar el usuario, además de otras tareas administrativas.

**Referencias**

Las referencias son los casos de uso que realiza el actor. En este caso, el administrador realiza los casos de uso "Alta y baja de usuarios", "Definir medio de transporte" y "Definir precio transporte". El usuario realiza los casos de uso "Definir destino", "Modificar ruta" y "Mostrar puntos de interés en ruta".

**Notas**

Las notas son información adicional sobre el actor. En este caso, la nota del administrador es "El administrador tiene acceso a todas las funcionalidades de la aplicación". La nota del usuario es "El usuario puede realizar tareas básicas para planificar sus viajes".

**Autor**

El autor es la persona que desarrolla la especificación del actor. En este caso, el autor es **Rafael Martín Mayor**.

**Fecha**

La fecha es la fecha de la especificación. En este caso, la fecha es **2024-01-28**.


## **Tabla de descripción de cada caso de uso**

| **Caso de uso** | **Actor principal** | **Precondiciones** | **Flujo principal** | **Postcondiciones** |
|---|---|---|---|---|
| **Definir medio de transporte** | Usuario | Tener una cuenta en la aplicación | El usuario selecciona el medio de transporte que desea utilizar | El sistema guarda el medio de transporte seleccionado |
| **Definir precio transporte** | Usuario | Tener una cuenta en la aplicación | El usuario introduce el precio del transporte seleccionado | El sistema guarda el precio del transporte seleccionado |
| **Alta y baja de usuarios** | Administrador | Tener acceso al sistema de administración | El administrador introduce los datos del usuario | El sistema crea o elimina el usuario |
| **Verificar credenciales** | Usuario | El usuario introduce sus credenciales | El sistema comprueba las credenciales del usuario | El sistema permite o deniega el acceso al usuario |
| **Login** | Usuario | Tener una cuenta en la aplicación | El usuario introduce sus credenciales | El sistema verifica las credenciales del usuario y permite el acceso a la aplicación |
| **Geoposicionamiento** | Sistema ext posic | El usuario ha iniciado sesión | El sistema ext posic obtiene la ubicación del usuario a través de un servicio externo | El sistema ext posic guarda la ubicación del usuario |
| **Definir destino** | Usuario | Tener una cuenta en la aplicación | El usuario introduce el destino al que desea viajar | El sistema guarda el destino del usuario |
| **Sugerir destinos interesantes** | Sistema | El usuario ha definido un destino | El sistema sugiere al usuario destinos interesantes cercanos | El sistema muestra al usuario una lista de destinos interesantes |
| **Mostrar puntos interés en ruta** | Sistema | El usuario ha definido un destino | El sistema muestra al usuario los puntos de interés en la ruta entre su ubicación y el destino | El sistema muestra al usuario una lista de puntos de interés |
| **Modificar ruta** | Usuario | Tener una cuenta en la aplicación | El usuario modifica el destino o la ruta | El sistema guarda los cambios realizados por el usuario |

**Explicación de los símbolos**

* **Actor principal:** El actor que inicia el caso de uso.
* **Precondiciones:** Condiciones que deben cumplirse antes de iniciar el caso de uso.
* **Flujo principal:** Descripción de los pasos que se realizan durante el caso de uso.
* **Postcondiciones:** Condiciones que se cumplen al finalizar el caso de uso.
* **<<include>>:** Caso de uso incluido.
* **<<extend>>:** Caso de uso extendido.

**Notas**

* El caso de uso **Definir destino** tiene dos extensiones: **Sugerir destinos interesantes** y **Mostrar puntos interés en ruta**. Estas extensiones se activan cuando el usuario pulsa los botones correspondientes.
* El caso de uso **Modificar ruta** puede incluir el caso de uso **Definir destino**. Esto significa que el usuario puede modificar tanto el destino como la ruta.


## **Tabla de especificación de casos de uso**

| Nombre | Precondición | Descripción | Secuencia normal | Postcondición | Excepciones | Solución |
|---|---|---|---|---|---|---|
| **Login** | El usuario debe tener una cuenta registrada en la aplicación. | El usuario inicia sesión en la aplicación introduciendo su nombre de usuario y contraseña. | 1. El usuario abre la aplicación. 2. El usuario introduce su nombre de usuario y contraseña. 3. El sistema verifica las credenciales del usuario. 4. Si las credenciales son correctas, el sistema permite al usuario iniciar sesión. 5. Si las credenciales son incorrectas, el sistema muestra un mensaje de error. | El usuario está autenticado en la aplicación. | - El usuario no tiene una cuenta registrada. - Las credenciales introducidas son incorrectas. | - El usuario crea una cuenta nueva. - El usuario comprueba sus credenciales. |
| **Definir destino** | El usuario debe estar autenticado en la aplicación. | El usuario define el destino de un trayecto. | 1. El usuario selecciona la opción "Definir destino". 2. El usuario introduce la dirección del destino. 3. El sistema muestra la ubicación del destino en el mapa. 4. El usuario confirma el destino. | El destino del trayecto está definido. | - El usuario no introduce una dirección válida. | - El usuario no confirma el destino. | El usuario introduce una dirección válida o cancela la operación. |
| **Sugerir destinos interesantes** | El usuario debe estar autenticado en la aplicación. | El sistema sugiere destinos interesantes para el usuario. | 1. El usuario selecciona la opción "Sugerir destinos interesantes". 2. El sistema sugiere una lista de destinos interesantes. 3. El usuario selecciona un destino de la lista. | El usuario tiene una lista de destinos interesantes para elegir. | - El sistema no encuentra destinos interesantes. | El sistema muestra un mensaje de error. | El usuario puede seleccionar un destino de la lista o cancelar la operación. |
| **Mostrar puntos de interés en ruta** | El usuario debe estar autenticado en la aplicación. | El sistema muestra los puntos de interés en la ruta del trayecto. | 1. El usuario selecciona la opción "Mostrar puntos de interés en ruta". 2. El sistema muestra una lista de puntos de interés en la ruta. 3. El usuario selecciona un punto de interés de la lista. | El usuario tiene una lista de puntos de interés en la ruta para elegir. | - El sistema no encuentra puntos de interés en la ruta. | El sistema muestra un mensaje de error. | El usuario puede seleccionar un punto de interés de la lista o cancelar la operación. |

**Explicación de las excepciones**

* **Excepción 1:** El usuario no tiene una cuenta registrada.

En este caso, el sistema muestra un mensaje de error que indica al usuario que debe crear una cuenta antes de iniciar sesión. El usuario puede crear una cuenta nueva seleccionando la opción "Registrarse".

* **Excepción 2:** Las credenciales introducidas son incorrectas.

En este caso, el sistema muestra un mensaje de error que indica al usuario que las credenciales introducidas son incorrectas. El usuario puede comprobar sus credenciales e intentar iniciar sesión nuevamente.

* **Excepción 3:** El usuario no introduce una dirección válida.

En este caso, el sistema muestra un mensaje de error que indica al usuario que la dirección introducida no es válida. El usuario puede introducir una dirección válida o cancelar la operación.

* **Excepción 4:** El sistema no encuentra destinos interesantes.

En este caso, el sistema muestra un mensaje de error que indica al usuario que no se han encontrado destinos interesantes. El usuario puede cancelar la operación.

* **Excepción 5:** El sistema no encuentra puntos de interés en la ruta.

En este caso, el sistema muestra un mensaje de error que indica al usuario que no se han encontrado puntos de interés en la ruta. El usuario puede cancelar la operación.

</div>