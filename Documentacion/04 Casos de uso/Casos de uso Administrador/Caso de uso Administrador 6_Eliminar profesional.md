**Caso de Uso: Eliminar profesional**

**Actor primario: Administrador**

**Precondiciones:**

* **El Administrador está autenticado en el sistema.**  
* **El Administrador tiene permisos para gestionar los profesionales.**  
* **Existe al menos un profesional registrado en el sistema.**

**Camino básico:**

1. **El usuario selecciona la opción "Eliminar profesional" desde el panel de administración.**  
2. **El sistema muestra la lista de profesionales registrados.**  
3. **El usuario selecciona uno o más profesionales que desea eliminar.**  
4. **El sistema habilita la eliminación y muestra un mensaje de confirmación "¿Está seguro de eliminar los profesionales seleccionados?".**  
5. **El usuario confirma la eliminación (presiona "Eliminar" o "Aceptar").**  
6. **El sistema elimina los profesionales seleccionados y muestra el mensaje: "Profesional(es) eliminado(s) correctamente".**

**Postcondiciones:**

* **Los profesionales seleccionados ya no están disponibles en el sistema.**  
* **No pueden ser asignados a nuevos turnos.**  
* **Los turnos existentes asignados a ellos permanecen intactos (o se cancelan/reasignan).**

**Caminos alternativos:**

**3a. Ningún profesional seleccionado**

**3a1. El sistema muestra el mensaje: "Debe seleccionar al menos un profesional para eliminar".**

**3a2. El sistema mantiene la lista visible.**

**3a3. El Administrador selecciona profesionales y vuelve a confirmar.**

**5a. El Administrador cancela la operación**

**5a1. El sistema cierra el diálogo de confirmación sin eliminar nada.**

**5a2. Regresa a la lista de profesionales (puede volver al paso 3 o al menú principal).**


**Escenario de éxito:**

**El administrador pudo eliminar el o los profesionales seleccionados con éxito. Los profesionales desaparecen de la lista y ya no aparecen como opción al asignar turnos.**

**Escenario de fracaso:**

**El administrador no pudo eliminar el o los profesionales debido a que no seleccionó ninguno o canceló la operación, y por lo tanto permanecen en el sistema sin cambios.**

