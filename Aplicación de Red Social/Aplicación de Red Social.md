<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

![](Aplicación%20de%20Red%20Social.drawio.png)

# Aplicación de Red Social

1. **Publicar Mensaje**
   - **Actor:** Usuario
   - **Pasos:**
     1. El usuario inicia sesión en la red social.
     2. Navega a la sección para crear una nueva publicación.
     3. Escribe el mensaje que desea compartir.
     4. Puede añadir multimedia si lo desea.
     5. Publica el mensaje en su perfil o en el muro general.

2. **Conectar con Amigos**
   - **Actor:** Usuario
   - **Pasos:**
     1. El usuario inicia sesión en la red social.
     2. Va a la opción de búsqueda o recomendaciones de amigos.
     3. Busca a un amigo específico o selecciona uno de la lista proporcionada.
     4. Envía una solicitud de amistad.
     5. Espera a que el amigo acepte la solicitud para estar conectados.

3. **Eliminar Publicación**
   - **Actor:** Administrador
   - **Pasos:**
     1. El administrador revisa las publicaciones reportadas o realiza un monitoreo regular.
     2. Selecciona una publicación que no cumple con las políticas de contenido.
     3. Elimina la publicación del muro o perfil donde está ubicada.

4. **Eliminar Usuario**
   - **Actor:** Administrador
   - **Pasos:**
     1. El administrador recibe reportes sobre un usuario, o detecta actividad inapropiada durante su monitoreo regular.
     2. Revisa las actividades y contenido asociado al usuario en cuestión para confirmar si violan las políticas del servicio.
     3. Si se confirma, procede a eliminar al usuario, desactivando su cuenta y eliminando todo su contenido asociado.


## **Tabla de descripción de cada actor:**

| Actor | Descripción | Características | Relaciones | Referencias | Autor | Fecha |
|---|---|---|---|---|---|---|
| **Usuario** | Persona que utiliza la red social para comunicarse con otros usuarios, compartir información y contenido, y participar en actividades sociales. | - Tiene una cuenta en la red social. - Puede crear publicaciones, comentarios y mensajes. - Puede conectarse con otros usuarios. - Puede participar en grupos y eventos. | Administrador | - **Casos de uso:** Publicar mensaje, Conectar con amigos | Rafael Martín Mayor | 2024-01-28 |
| **Administrador** | Persona encargada de administrar la red social, asegurando su correcto funcionamiento y cumplimiento de las políticas y normas establecidas. | - Tiene acceso a la información y datos de la red social. - Puede administrar las cuentas de usuario. - Puede crear y gestionar contenido. - Puede moderar las publicaciones y comentarios. | Usuario | - **Casos de uso:** Eliminar usuario, Eliminar publicación | Rafael Martín Mayor | 2024-01-28 |

## **Tabla de especificación de casos de uso:**

| **Caso de Uso** | **Actores** | **Descripción** | **Precondición** | **Secuencia normal** | **Postcondición** | **Excepciones con solución** | **Autor** | **Fecha** |
|---|---|---|---|---|---|---|---|---|
| **Publicar mensaje** | **Usuario** | El usuario publica un mensaje en la red social. | El usuario está registrado en la red social. | 1. El usuario selecciona la opción "Publicar mensaje". 2. El sistema muestra un formulario para crear el mensaje. 3. El usuario llena el formulario con el contenido del mensaje. 4. El usuario selecciona la opción "Publicar". 5. El sistema publica el mensaje en la red social. | El mensaje se publica en la red social y es visible para todos los usuarios. | - **El mensaje es demasiado largo o tiene contenido inapropiado.** Solución: El sistema muestra un mensaje de error y el usuario debe reducir el tamaño del mensaje y/o quitar el contenido inapropiado. | Rafael Martín Mayor | 2024-01-28 |
| **Conectar con amigos** | **Usuario** | El usuario se conecta con otro usuario en la red social. | El usuario está registrado en la red social. | 1. El usuario selecciona la opción "Conectar con amigos". 2. El sistema muestra una lista de usuarios. 3. El usuario selecciona el usuario con el que quiere conectarse. 4. El sistema envía una solicitud de conexión al usuario seleccionado. 5. El usuario seleccionado puede aceptar o rechazar la solicitud. | El usuario está conectado con el usuario seleccionado. | - **El usuario seleccionado no existe.** Solución: El sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |
| **Eliminar publicación** | **Administrador** | El administrador elimina la publicación de un usuario. | El administrador considera la publicación inapropiada. | 1. El administrador selecciona la publicación que quiere eliminar. 2. El sistema muestra un mensaje de confirmación. 3. El administrador selecciona la opción "Eliminar". 4. El sistema elimina la publicación. | La publicación es eliminada de la red social. | - **La publicación no existe.** Solución: El sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |
| **Eliminar usuario** | **Administrador** | El administrador elimina una cuenta de usuario de la red social. | El administrador considera que la conducta del usuario en cuestión ha infiringido las normas de la red social y debe ser eliminado. | 1. El administrador selecciona la cuenta de usuario que quiere eliminar. 2. El sistema muestra un mensaje de confirmación. 3. El administrador selecciona la opción "Eliminar". 4. El sistema elimina la cuenta de usuario. | La cuenta de usuario es eliminada de la red social. | - **La cuenta de usuario no existe.** Solución: El sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |

</div>