Rafael Martín Mayor.

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

    1. Mostrar puntos de interés en la ruta: El sistema externo de posicionamiento puede mostrar puntos de interés en la ruta sugerida por la aplicación.
