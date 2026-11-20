## Caso de Uso: Eliminar profesional

**Actor primario:** Administrador

**Precondiciones:**

- El Administrador está autenticado en el sistema.
- El Administrador tiene permisos para gestionar los profesionales.
- Existe al menos un profesional registrado en el sistema.

**Camino básico:**

1. **El usuario** solicita eliminar uno o más profesionales del sistema.
2. **El sistema** consulta y proporciona la lista de profesionales registrados.
3. **El usuario** selecciona los profesionales que desea eliminar.
4. **El sistema** solicita la confirmación de la operación.
5. **El usuario** confirma la eliminación de los profesionales seleccionados.
6. **El sistema** elimina los profesionales del sistema y confirma que la operación se realizó correctamente.

**Postcondiciones:**

- Los profesionales seleccionados dejan de estar disponibles en el sistema.
- Los profesionales eliminados ya no pueden ser asignados a nuevos turnos.
- Los turnos existentes asociados a los profesionales permanecen sujetos a las reglas de gestión de turnos del sistema.

**Caminos alternativos:**

**3a. Ningún profesional seleccionado**

3a1. **El sistema** informa que debe seleccionarse al menos un profesional para continuar con la eliminación.

3a2. **El usuario** selecciona uno o más profesionales.

3a3. **El sistema** valida la selección y solicita la confirmación de la operación.

**5a. El usuario cancela la operación**

5a1. **El usuario** cancela la eliminación de los profesionales seleccionados.

5a2. **El sistema** cancela la operación y conserva los profesionales sin realizar modificaciones.

**Escenario de éxito:**

El administrador elimina correctamente uno o más profesionales y el sistema los quita del registro, impidiendo que sean asignados a nuevos turnos.

**Escenario de fracaso:**

El sistema no elimina los profesionales debido a que no se seleccionó ninguno o porque el administrador canceló la operación. Los profesionales permanecen registrados sin modificaciones.