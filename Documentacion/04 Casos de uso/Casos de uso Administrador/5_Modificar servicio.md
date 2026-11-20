## Caso de Uso: Modificar servicio

**Actor primario:** Administrador

**Precondiciones:**

- El Administrador está autenticado en el sistema.
- El Administrador tiene permisos para gestionar el catálogo de servicios.
- Existe al menos un servicio registrado en el catálogo.

**Camino básico:**

1. **El usuario** solicita modificar un servicio del catálogo.
2. **El sistema** consulta y proporciona la lista de servicios registrados.
3. **El usuario** selecciona el servicio que desea modificar.
4. **El sistema** proporciona los datos actuales del servicio seleccionado.
5. **El usuario** modifica los datos necesarios del servicio.
6. **El sistema** valida que los campos obligatorios estén completos y que los datos ingresados sean correctos, incluyendo que el precio sea mayor a cero.
7. **El usuario** confirma los cambios realizados.
8. **El sistema** actualiza los datos del servicio en el catálogo y confirma que la modificación se realizó correctamente.

**Postcondiciones:**

- El servicio queda actualizado en el catálogo con los nuevos datos.
- Los cambios quedan disponibles para los clientes al solicitar nuevos turnos.

**Caminos alternativos:**

**3a. Ningún servicio seleccionado**

3a1. **El sistema** informa que debe seleccionarse un servicio para continuar con la modificación.

3a2. **El usuario** selecciona el servicio que desea modificar.

3a3. **El sistema** proporciona los datos actuales del servicio seleccionado.

**6a. Datos modificados inválidos o incompletos**

6a1. **El sistema** informa que los datos ingresados son inválidos o están incompletos.

6a2. **El usuario** corrige los datos solicitados.

6a3. **El sistema** valida nuevamente los datos ingresados.

**7a. El usuario cancela los cambios**

7a1. **El usuario** cancela la modificación del servicio.

7a2. **El sistema** cancela la operación y conserva los datos originales sin realizar modificaciones.

**Escenario de éxito:**

El administrador modifica correctamente el servicio y el sistema actualiza sus datos en el catálogo, dejando disponibles los nuevos valores para los clientes.

**Escenario de fracaso:**

El sistema no modifica el servicio debido a datos inválidos, incompletos o a la cancelación de la operación. El servicio permanece registrado con sus datos originales.