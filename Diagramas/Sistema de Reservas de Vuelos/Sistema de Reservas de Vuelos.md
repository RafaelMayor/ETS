<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

## Diagrama de casos de uso de Sistema de Reservas de Vuelos:

![](Sistema%20de%20Reservas%20de%20Vuelos.drawio.png)

## Diagrama de secuencia de Sistema de Reservas de Vuelos:

![](DS%20Sistema%20de%20Reservas%20de%20Vuelos.drawio.png)

## Diagrama de actividades de Sistema de Reservas de Vuelos:

![](DAct%20Sistema%20de%20Reservas%20de%20Vuelos.png)

## Diagrama de clases de Sistema de Reservas de Vuelos:

![](DC%20Sistema%20de%20Reservas%20de%20Vuelos.png)

## Sistema de Reservas de Vuelos

### 1. Reservar Vuelo
   - **Actor:** Pasajero, Agente de Reservas
   - **Descripción:** Permite a los usuarios reservar un vuelo seleccionando la fecha, hora y destino deseados.
   - **Pasos:**
   1. El pasajero solicita una reserva.
   2. El agente de reservas inicia el proceso de reserva.
   3. Selecciona la fecha, hora y destino del vuelo.
   4. El sistema muestra las opciones disponibles.
   5. El usuario selecciona un vuelo específico.
   6. Se completa la información del pasajero y se procede al pago.
   7. El sistema confirma la reserva.

### 2. Cancelar Reserva
   - **Actor:** Pasajero, Agente de Reservas
   - **Descripción:** Permite a los usuarios cancelar una reserva existente.
   - **Pasos:**
   1. El pasajero solicita cancelar una reserva.
   2. El agente de reservas selecciona la opción para cancelar una reserva existente.
   3. Se solicita la información de la reserva.
   4. El sistema muestra los detalles de la reserva.
   5. El usuario confirma la cancelación.
   6. El sistema procesa la cancelación y notifica al usuario.

### 3. Cambiar Vuelo
   - **Actor:** Pasajero, Agente de Reservas
   - **Descripción:** Permite a los usuarios modificar los detalles de un vuelo reservado previamente.
   - **Pasos:**
   1. El pasajero opta por cambiar un vuelo ya reservado.
   2. El agente de reservas introduce los detalles de la reserva existente.
   3. Seleccionan nuevas opciones para fecha, hora o destino del vuelo según sea necesario.
   4. El sistema muestra las opciones disponibles.
   5. El usuario selecciona un vuelo específico.
   6. Se completa la información del pasajero y se procede al pago.
   7. El sistema confirma la reserva.

### 4. Buscar Vuelo
   - **Actor:** Agente de Reservas
   - **Descripción:** El Agente de Reservas busca vuelos disponibles según las preferencias del Pasajero.
   - **Pasos:**
   1. El agente de reservas selecciona la opción para buscar vuelos.
   2. Seleccionan la fecha, hora y destino del vuelo.
   3. El sistema muestra las opciones disponibles.

## **Tabla de descripción de cada actor:**

| Actor | Descripción | Características | Relaciones | Referencias | Autor | Fecha |
|---|---|---|---|---|---|---|
| **Pasajero** | Persona que desea realizar un viaje en avión. | Persona física, con nombre y apellidos, DNI o pasaporte, dirección, etc. | **Agente de Reservas** | **Reservar Vuelo**, **Cancelar Reserva**, **Cambiar Vuelo** | Rafael Martín Mayor | 2024-01-28 |
| **Agente de Reservas** | Persona que trabaja para una aerolínea y se encarga de realizar reservas de vuelos. | Persona física, con nombre y apellidos, DNI o pasaporte, dirección, etc. | **Pasajero** | **Reservar Vuelo**, **Cancelar Reserva**, **Cambiar Vuelo**, **Buscar Vuelo** | Rafael Martín Mayor | 2024-01-28 |

## **Tabla de especificación de casos de uso:**

| Caso de Uso | Actores | Descripción | Precondición | Secuencia normal | Postcondición | Excepciones con solución | Autor | Fecha |
|---|---|---|---|---|---|---|---|---|
| **Reservar Vuelo** | Pasajero, Agente de Reservas | El pasajero solicita la reserva de un vuelo. | El pasajero está registrado en el sistema. El vuelo que se desea reservar está disponible. | 1. El pasajero inicia el caso de uso. 2. El pasajero proporciona los datos del vuelo que desea reservar. 3. El agente de reservas verifica la disponibilidad del vuelo. 4. El agente de reservas confirma la reserva del vuelo. 5. El sistema genera un número de reserva. 6. El pasajero finaliza el caso de uso. | El sistema debe almacenar la información de la reserva. El sistema debe notificar al pasajero de la reserva. | El vuelo se encuentra agotado. El pasajero proporciona datos de vuelo incorrectos. El sistema debe mostrar un mensaje de error al pasajero. El sistema debe permitir al pasajero volver a intentar la reserva. | Rafael Martín Mayor | 2024-01-28 |
| **Cancelar Reserva** | Pasajero, Agente de Reservas | El pasajero cancela una reserva de vuelo. | El pasajero tiene una reserva de vuelo activa. | 1. El pasajero inicia el caso de uso. 2. El pasajero proporciona el número de reserva. 3. El agente de reservas verifica la reserva. 4. El agente de reservas confirma la cancelación de la reserva. 5. El sistema elimina la reserva. 6. El pasajero finaliza el caso de uso. | El sistema debe eliminar la reserva de vuelo. El sistema debe notificar al pasajero de la cancelación. | El número de reserva es incorrecto. La reserva ya ha sido cancelada. El sistema debe mostrar un mensaje de error al pasajero. | Rafael Martín Mayor | 2024-01-28 |
| **Cambiar Vuelo** | Pasajero, Agente de Reservas | El pasajero cambia los datos de una reserva de vuelo. | El pasajero tiene una reserva de vuelo activa. | 1. El pasajero inicia el caso de uso. 2. El pasajero proporciona el número de reserva y los datos que desea cambiar. 3. El agente de reservas verifica la reserva. 4. El agente de reservas confirma el cambio de datos. 5. El sistema actualiza la reserva. 6. El pasajero finaliza el caso de uso. | El sistema debe actualizar la reserva de vuelo. El sistema debe notificar al pasajero del cambio. | El número de reserva es incorrecto. Los datos que se desean cambiar son incorrectos. El sistema debe mostrar un mensaje de error al pasajero. | Rafael Martín Mayor | 2024-01-28 |
| **Buscar Vuelo** | Agente de Reservas | El agente de reservas busca vuelos disponibles. | No hay precondiciones. | 1. El agente de reservas inicia el caso de uso. 2. El agente de reservas proporciona los criterios de búsqueda. 3. El sistema recupera los vuelos que cumplen los criterios. 4. El agente de reservas finaliza el caso de uso. | El sistema debe devolver una lista de vuelos que cumplan los criterios. | El sistema debe proporcionar una interfaz de búsqueda intuitiva. | Rafael Martín Mayor | 2024-01-28 |

</div>