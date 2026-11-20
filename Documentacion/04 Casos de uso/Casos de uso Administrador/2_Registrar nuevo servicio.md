## Caso de Uso: Registrar nuevo servicio

**Actor primario:** Administrador

**Precondiciones:**

- El Administrador está autenticado en el sistema.
- El Administrador tiene permisos para gestionar el catálogo de servicios.

**Camino básico:**

1. **El usuario** ingresa el nombre y el precio del servicio.
2. **El sistema** valida que los campos estén completos, que el precio sea mayor a cero y que no exista otro servicio con el mismo nombre.
3. **El usuario** confirma el registro del nuevo servicio.
4. **El sistema** registra el servicio en el catálogo y confirma que el registro se realizó correctamente.

**Postcondiciones:**

- El nuevo servicio queda registrado en el catálogo del sistema.
- El servicio queda disponible para ser seleccionado por los clientes al solicitar turnos.

**Caminos alternativos:**

**4a. Datos inválidos o incompletos**

4a1. **El sistema** informa que los datos ingresados son inválidos o están incompletos.

4a2. **El usuario** corrige los datos solicitados.

4a3. **El sistema** valida nuevamente los datos ingresados.

**4b. Nombre de servicio ya existente**

4b1. **El sistema** informa que ya existe un servicio registrado con ese nombre.

4b2. **El usuario** modifica el nombre del servicio.

4b3. **El sistema** valida nuevamente el nombre ingresado y continúa con el proceso de registro si está disponible.

**Escenario de éxito:**

El administrador registra correctamente el nuevo servicio y el sistema lo incorpora al catálogo, dejándolo disponible para los clientes.

**Escenario de fracaso:**

El sistema no registra el servicio debido a datos inválidos, incompletos o a la existencia de otro servicio con el mismo nombre.