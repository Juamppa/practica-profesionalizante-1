## Caso de Uso: Eliminar servicio

**Actor primario:** Administrador

**Precondiciones:**

- El Administrador está autenticado en el sistema.
- El Administrador tiene permisos para gestionar el catálogo de servicios.
- Existe al menos un servicio registrado en el catálogo.

**Camino básico:**

1. **El usuario** solicita eliminar uno o más servicios del catálogo.
2. **El sistema** consulta y proporciona la lista de servicios registrados.
3. **El usuario** selecciona los servicios que desea eliminar.
4. **El sistema** solicita la confirmación de la operación.
5. **El usuario** confirma la eliminación de los servicios seleccionados.
6. **El sistema** elimina los servicios del catálogo y confirma que la operación se realizó correctamente.

**Postcondiciones:**

- Los servicios seleccionados dejan de estar disponibles en el catálogo.
- Los servicios eliminados ya no pueden ser seleccionados por los clientes al solicitar nuevos turnos.

**Caminos alternativos:**

**3a. Ningún servicio seleccionado**

3a1. **El sistema** informa que debe seleccionarse al menos un servicio para continuar con la eliminación.

3a2. **El usuario** selecciona uno o más servicios.

3a3. **El sistema** valida la selección y solicita la confirmación de la operación.

**5a. El usuario cancela la operación**

5a1. **El usuario** cancela la eliminación de los servicios seleccionados.

5a2. **El sistema** cancela la operación y conserva los servicios sin realizar modificaciones.

**Escenario de éxito:**

El administrador elimina correctamente uno o más servicios y el sistema los quita del catálogo, impidiendo que sean seleccionados por los clientes al solicitar nuevos turnos.

**Escenario de fracaso:**

El sistema no elimina los servicios debido a que no se seleccionó ninguno o porque el administrador canceló la operación. Los servicios permanecen registrados en el catálogo.