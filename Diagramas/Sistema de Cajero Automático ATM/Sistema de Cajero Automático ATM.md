<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

## Diagrama de casos de uso de Sistema de Cajero Automático ATM:

![](Sistema%20de%20Cajero%20Automático%20ATM.drawio.png)

## Diagrama de secuencia de Sistema de Cajero Automático ATM:

![](DS%20Sistema%20cajero%20automatico%20Rafa.jpg)

## Diagrama de actividades de Sistema de Cajero Automático ATM:

![](DAct%20Sistema%20cajero%20automatico.png)

## Diagrama de clases de Sistema de Cajero Automático ATM:

![](DAct%20Sistema%20cajero%20automatico.png)

# Sistema de Cajero Automático ATM


1. **Hacer login:**
   - **Actor:** Cliente Bancario
   - **Pasos:**
     1. El cliente se acerca al cajero automático.
     2. Introduce su tarjeta o realiza una identificación biométrica.
     3. Ingresa su PIN o contraseña para acceder a los servicios del cajero.

2. **poner dinero al móvil: («extend» de Hacer login)**
   - **Actor:** Cliente Bancario
   - **Pasos:**
     1. El cliente selecciona la opción "Poner dinero al móvil" después de hacer login.
     2. Ingresa el número de teléfono y la cantidad a transferir.
     3. Confirma la transacción.

3. **Realizar transferencia: («extend» de Hacer login)**
   - **Actor:** Cliente Bancario
   - **Pasos:**
     1. Selecciona la opción "Realizar transferencia".
     2. Ingresa los detalles de la cuenta destinataria y el monto a transferir.
     3. Confirma los detalles y completa la transacción.

4. **Ingresar dinero: («extend» de Hacer login)** 
   - **Actor:** Cliente Bancario
   - **Pasos:**
     1. Selecciona “Ingresar dinero” en el menú del cajero automático.
     2. Inserta las notas o monedas en las ranuras correspondientes.
     3. Confirma la cantidad ingresada y finaliza la transacción.

5. **ver Saldo («extend» de Hacer login)**
   - **Actor:** Cliente Bancario
   - **Pasos:**
     1. El cliente se acerca al cajero automático.
     2. Inserta su tarjeta o realiza el login con sus credenciales.
     3. Selecciona la opción "ver saldo" en la interfaz del cajero.
     4. El cajero muestra el saldo actual en la pantalla.

6. **Reparar Cajero**
   - **Actor:** Administrador
   - **Pasos:**
     1. El administrador recibe una notificación de un cajero defectuoso o realiza una inspección rutinaria y detecta un problema.
     2. Se acerca al cajero automático afectado.
     3. Utiliza herramientas y conocimientos técnicos para diagnosticar el problema específico del cajero.
     4. Repara el cajero, que puede incluir reemplazar piezas defectuosas, actualizar el software o corregir problemas mecánicos/electrónicos.


## **Tabla de descripción de cada actor:**

| Actor | Descripción | Características | Relaciones | Referencias | Autor | Fecha |
|---|---|---|---|---|---|---|
| **Cliente Bancario** | Persona que tiene una cuenta bancaria en el sistema. | Tiene una cuenta bancaria en el sistema. Tiene una tarjeta de débito o crédito. Tiene un dispositivo móvil. | Administrador | Hacer login, poner dinero en el móvil, Realizar transferencia, Ingresar dinero y ver saldo. | Rafael Martín Mayor | **Fecha:** 2024-01-28 |
| **Administrador** | Persona que tiene privilegios de administrador del sistema. | Tiene acceso a la base de datos del sistema. Puede realizar cambios en el sistema. | Cliente Bancario | Reparar cajero. | Rafael Martín Mayor | 2024-01-28 |

## **Tabla de especificación de casos de uso:**

| Caso de uso | Actores | Descripción | Precondición | Secuencia normal | Postcondición | Excepciones | Autor | Fecha |
|---|---|---|---|---|---|---|---|---|
| **Hacer login** | Cliente Bancario | El cliente bancario inicia sesión en el sistema. | El cliente bancario tiene una cuenta bancaria registrada en el sistema. | 1. El cliente bancario introduce sus credenciales de acceso. 2. El sistema verifica las credenciales de acceso. 3. El sistema permite al cliente bancario iniciar sesión. | El cliente bancario ha iniciado sesión con éxito en el sistema. | Si las credenciales de acceso son incorrectas, el sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |
| **poner dinero al móvil** | Cliente bancario | El cliente bancario puede recargar su saldo móvil. | El cliente bancario está registrado en el sistema y tiene una cuenta bancaria. | 1. El cliente bancario introduce sus datos de acceso. 2. El sistema verifica los datos de acceso del cliente bancario. 3. El cliente bancario introduce el número de teléfono móvil. 4. El cliente bancario introduce el importe de la recarga. 5. El sistema verifica que el importe de la recarga es válido. 6. El sistema realiza la recarga. 7. El sistema muestra un mensaje de confirmación. | La recarga se realiza correctamente. | * El cliente bancario no está registrado en el sistema. El sistema muestra un mensaje de error. * El cliente bancario no tiene una cuenta bancaria. El sistema muestra un mensaje de error. * El importe de la recarga es inválido. El sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |
| **Realizar transferencia** | Cliente bancario | El cliente bancario puede realizar una transferencia de dinero entre sus cuentas o a una cuenta de un tercero. | El cliente bancario está registrado en el sistema y tiene acceso a una cuenta bancaria. | 1. El cliente bancario introduce sus datos de acceso. 2. El sistema verifica los datos de acceso del cliente bancario. 3. El cliente bancario selecciona la cuenta de origen y la cuenta de destino. 4. El cliente bancario introduce el importe de la transferencia. 5. El sistema verifica que el importe de la transferencia es válido. 6. El sistema realiza la transferencia. 7. El sistema muestra un mensaje de confirmación. | La transferencia se realiza correctamente. | * El cliente bancario no está registrado en el sistema. El sistema muestra un mensaje de error. * El cliente bancario no tiene acceso a una cuenta bancaria. El sistema muestra un mensaje de error. * El importe de la transferencia es inválido. El sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |
| **Ingresar dinero** | Cliente bancario | El cliente bancario ingresa dinero en su cuenta. | El cliente debe tener dinero que sea válido. | 1. El cliente selecciona la opción "Ingresar dinero" del menú. 2. El cliente introduce la cantidad de dinero a ingresar. 3. El cliente confirma el ingreso. 4. El sistema verifica la cantidad de dinero. 5. El sistema registra el ingreso en la cuenta del cliente. | El dinero se ha ingresado correctamente en la cuenta del cliente. | El cliente introduce dinero falso. El sistema muestra un mensaje de error y solicita al cliente que introduzca dinero válido. El cliente no introduce una cantidad de dinero válida. El sistema muestra un mensaje de error y solicita al cliente que introduzca una cantidad válida. | Rafael Martín Mayor | 2024-01-28 |
| **Ver saldo** | Cliente bancario | El cliente bancario puede consultar su saldo bancario. | El cliente bancario está registrado en el sistema y tiene acceso a una cuenta bancaria. | 1. El cliente bancario introduce sus datos de acceso. 2. El sistema verifica los datos de acceso del cliente bancario. 3. El sistema muestra el saldo de la cuenta bancaria del cliente bancario. | El cliente bancario puede ver su saldo bancario. | * El cliente bancario no está registrado en el sistema. El sistema muestra un mensaje de error. * El cliente bancario no tiene acceso a una cuenta bancaria. El sistema muestra un mensaje de error. | Rafael Martín Mayor | 2024-01-28 |
| **Reparar cajero** | Administrador | El administrador puede reparar un cajero automático que está averiado. | El cajero automático está averiado. | 1. El administrador identifica el cajero automático averiado. 2. El administrador accede al cajero automático. 3. El administrador realiza las reparaciones necesarias. 4. El administrador verifica que el cajero automático funciona correctamente. | El cajero automático está reparado. | * El cajero automático no está averiado. El administrador no realiza ninguna acción. | Rafael Martín Mayor | 2024-01-28 |

</div>