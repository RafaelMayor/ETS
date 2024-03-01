<div align="justify">

<div align="right">
Rafael Martín Mayor.
</div>

# Diagrama de clases de un Club Náutico:

![](DC%20Club%20Náutico.png)

# Club Náutico


1. **Clase Socio:**
   - **Definición:** La clase "Socio" representa a una persona o entidad que es miembro de un club náutico o puerto deportivo. Los socios pueden ser propietarios de embarcaciones y tienen ciertos derechos y responsabilidades dentro de la organización.
   - **Atributos:**
     - `nombre`: El nombre del socio.
     - `dirección`: La dirección de residencia o negocio del socio.
     - `DNI`: El número de identificación personal del socio.
     - `teléfono`: El número de teléfono de contacto del socio.
     - `fechaIngreso`: La fecha en la que el socio se unió al club.
   - **Relaciones:**
     - Es Propietario de cero o más embarcaciones.
     - Puede tener cero o más amarres.
   - **Cardinalidad:**
     - La relación con las embarcaciones es de 0 o más (0-*).
     - La relación con los empleados también es de 0 o más (0-*).

2. **Clase Embarcación:**
   - **Definición:** Representa una embarcación, ya sea un barco, velero o cualquier otra nave. Las embarcaciones pueden ser propiedad de un socio y están ancladas en los amarres del puerto.
   - **Atributos:**
     - `matrícula`: La matrícula o registro oficial de la embarcación.
     - `nombre`: El nombre de la embarcación.
     - `tipo`: El tipo de embarcación (por ejemplo, velero, lancha, etc.).
     - `dimensiones`: Las dimensiones físicas de la embarcación (longitud, ancho, etc.).
   - **Relaciones:**
     - "EsPropietario" por un socio.
     - Ocupa un amarre específico.
   - **Cardinalidad:**
     - Cada embarcación tiene un propietario (1-1).
     - Ocupa un amarre (1-1).

3. **Clase Amarre:**
   - **Definición:** Representa un espacio físico en el puerto donde se atracan las embarcaciones. Los amarres pueden tener servicios como agua, electricidad y mantenimiento.
   - **Atributos:**
     - `numeroAmarre`: Número único que identifica el amarre.
     - `contadorAgua`: Registro del consumo de agua en el amarre.
     - `contadorLuz`: Registro del consumo de electricidad en el amarre.
     - `serviciosMantenimiento`: Indica si se realizan servicios de mantenimiento en el amarre.
   - **Relaciones:**
     - Es "ocupado" por una embarcación específica.
     - "Pertenece a" una zona del puerto.
     - Es propia de un propietario.
   - **Cardinalidad:**
     - Cada amarre está ocupado por una embarcación (1-1).
     - Pertenece a una zona (1-1).
     - Es propia de un propietario (1-1).

4. **Clase Empleado:**
   - **Definición:** Representa a un empleado del club náutico o puerto deportivo. Los empleados pueden desempeñar diversas funciones, como atención al cliente, mantenimiento o seguridad.
   - **Atributos:**
     - `código`: Identificador único del empleado.
     - `nombre`: Nombre del empleado.
     - `dirección`: Dirección de residencia del empleado.
     - `teléfono`: Número de teléfono de contacto del empleado.
     - `especialidad`: Área de especialización o función del empleado.
   - **Relaciones:**
     - Es "asignado a" dos o más zonas para brindar asistencia.
   - **Cardinalidad:**
     - La relación con la clase Zona tiene una cardinalidad de "2-*" indicando que cada empleado puede ser asignado a dos o más zonas.

5. **Clase Zona:**
   - **Definición:** La clase "Zona" representa una sección específica dentro del puerto o club náutico. Cada zona tiene características particulares que afectan la operación y el uso de las instalaciones.
   - **Atributos:**
     - `letra`: Identifica la zona mediante una letra (por ejemplo, "A", "B", etc.). Esta letra puede ser útil para la organización y referencia.
     - `tipoBarcos`: Indica el tipo de barcos que pueden anclarse en esta zona. Por ejemplo, algunas zonas pueden estar designadas para veleros, mientras que otras pueden ser para lanchas motoras.
     - `numeroBarcos`: Representa el número total de barcos que pueden ser anclados en esta zona. Esto ayuda a controlar la capacidad y evitar la congestión.
     - `profundidad`: Indica la profundidad del agua en esta zona. Algunas zonas pueden ser más profundas y adecuadas para embarcaciones más grandes, mientras que otras pueden ser más someras.
     - `anchoAmarres`: Describe el ancho de los amarres en la zona. Esto es importante para asegurar que las embarcaciones puedan atracar cómodamente sin restricciones de espacio.
   - **Relaciones:**
     - Le pertenece 2 o más amarres.
       - Cardinalidad: A una zona le puede pertenecer 2 o más amarres.
     - Es asignada a un empleado.
       - Cardinalidad: Cada zona puede ser asignada a uno o más empleados.


</div>