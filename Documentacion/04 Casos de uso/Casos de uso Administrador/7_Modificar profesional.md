## Caso de Uso: Modificar profesional

**Actor primario:** Administrador

**Precondiciones:**

- El Administrador está autenticado en el sistema.
- El Administrador tiene permisos para gestionar los profesionales.
- Existe al menos un profesional registrado en el sistema.

**Camino básico:**

1. **El usuario** solicita modificar un profesional registrado en el sistema.
2. **El sistema** consulta y proporciona la lista de profesionales registrados.
3. **El usuario** selecciona el profesional que desea modificar.
4. **El sistema** proporciona los datos actuales del profesional seleccionado.
5. **El usuario** modifica los datos necesarios del profesional, como nombre, apellido y disponibilidad.
6. **El sistema** valida que los campos obligatorios estén completos y que los datos ingresados tengan formatos correctos.
7. **El usuario** confirma los cambios realizados.
8. **El sistema** actualiza los datos del profesional y confirma que la modificación se realizó correctamente.

**Postcondiciones:**

- El profesional queda actualizado con los nuevos datos.
- Los cambios quedan disponibles para la asignación de nuevos turnos.

**Caminos alternativos:**

**3a. Ningún profesional seleccionado**

3a1. **El sistema** informa que debe seleccionarse un profesional para continuar con la modificación.

3a2. **El usuario** selecciona el profesional que desea modificar.

3a3. **El sistema** proporciona los datos actuales del profesional seleccionado.

**6a. Datos modificados inválidos o incompletos**

6a1. **El sistema** informa que los datos ingresados son inválidos o están incompletos.

6a2. **El usuario** corrige los datos solicitados.

6a3. **El sistema** valida nuevamente los datos ingresados.

**7a. El usuario cancela los cambios**

7a1. **El usuario** cancela la modificación del profesional.

7a2. **El sistema** cancela la operación y conserva los datos originales sin realizar modificaciones.

**Escenario de éxito:**

El administrador modifica correctamente los datos del profesional y el sistema actualiza su información, dejando disponibles los nuevos datos para la asignación de turnos.

**Escenario de fracaso:**

El sistema no modifica al profesional debido a datos inválidos, incompletos o a la cancelación de la operación. El profesional permanece registrado con sus datos originales.