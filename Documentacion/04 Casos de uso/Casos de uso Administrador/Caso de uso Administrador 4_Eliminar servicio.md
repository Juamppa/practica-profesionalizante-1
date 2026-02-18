**Caso de Uso: Eliminar servicio**

**Actor primario: Administrador**

**Precondiciones:**

* **El Administrador está autenticado en el sistema.**   
* **El Administrador tiene permisos para gestionar el catálogo de servicios.**  
* **Existe al menos un servicio registrado en el catálogo.**

**Camino básico:**

1. **El usuario selecciona la opción "Eliminar servicio" desde el panel de administración.**  
2. **El sistema muestra la lista de servicios disponibles en el catálogo.**  
3. **El usuario selecciona uno o más servicios que desea eliminar.**  
4. **El sistema habilita el botón de eliminación y muestra un mensaje de confirmación (ej. "¿Está seguro de eliminar los servicios seleccionados?").**  
5. **El usuario confirma la eliminación (presiona "Eliminar" o "Aceptar").**  
6. **El sistema elimina los servicios seleccionados del catálogo y muestra el mensaje: "Servicio(s) eliminado(s) correctamente".**

**Postcondiciones:**

* **Los servicios seleccionados ya no están disponibles en el catálogo.**  
* **No pueden ser seleccionados por clientes al solicitar nuevos turnos.**

**Caminos alternativos:**

**3a. Ningún servicio seleccionado**

**3a1. El sistema muestra un mensaje: "Debe seleccionar al menos un servicio para eliminar".**

**3a2. El sistema mantiene la lista visible.**

**3a3. El Administrador selecciona servicios y vuelve a confirmar.**

**5a. El Administrador cancela la operación.**

**5a1. El sistema cierra el diálogo de confirmación sin eliminar nada.**

**5a2. Regresa a la lista de servicios (puede volver al paso 3 o al menú principal).**

**Escenario de éxito:**

**El administrador pudo eliminar el o los servicios seleccionados con éxito. Los servicios desaparecen del catálogo y ya no aparecen como opción al solicitar turnos para los clientes.**

**Escenario de fracaso:**

**El administrador no pudo eliminar el o los servicios debido a que no seleccionó ninguno o canceló la operación, y por lo tanto los servicios permanecen en el catálogo sin cambios.**

