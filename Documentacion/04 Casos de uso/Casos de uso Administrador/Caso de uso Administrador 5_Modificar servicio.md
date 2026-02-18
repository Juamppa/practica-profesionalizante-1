**Caso de Uso: Modificar servicio**

**Actor primario: Administrador**

**Precondiciones:**

* **El Administrador está autenticado en el sistema.**   
* **El Administrador tiene permisos para gestionar el catálogo de servicios.**  
* **Existe al menos un servicio registrado en el catálogo.**

**Camino básico:**

1. **El usuario selecciona la opción "Modificar servicio" desde el panel de administración.**  
2. **El sistema muestra la lista de servicios disponibles en el catálogo.**  
3. **El usuario selecciona el servicio que desea modificar.**  
4. **El sistema muestra el formulario con los datos actuales del servicio precargados.**  
5. **El usuario modifica los campos necesarios (por ejemplo, precio, nombre, duración, etc.).**  
6. **El sistema valida los datos modificados (campos obligatorios completos, precio \> 0, etc.).**  
7. **El usuario presiona "Aceptar" para confirmar los cambios.**  
8. **El sistema actualiza el servicio en el catálogo y muestra el mensaje: "Servicio modificado correctamente".**

**Postcondiciones:**

* **El servicio queda actualizado en el catálogo con los nuevos datos.**  
* **Los cambios se reflejan inmediatamente en las opciones disponibles para los clientes al solicitar turnos.**

**Caminos alternativos:**

**3a. Ningún servicio seleccionado**

**3a1. El sistema muestra un mensaje: "Debe seleccionar al menos un servicio para modificar".**

**3a2. El sistema mantiene la lista visible.**

**3a3. El Administrador selecciona un servicio y continúa.**

**5a/6a. Datos modificados inválidos o incompletos.**

**6a1. El sistema muestra mensajes de error específicos junto a los campos problemáticos (ej. "Precio debe ser mayor a 0").**

**6a2. El sistema mantiene el formulario abierto con los cambios parciales.**

**6a3. El Administrador corrige los datos y vuelve a confirmar.**

**7a. El Administrador cancela los cambios**

**7a1. El sistema cierra el formulario sin guardar nada.**

**7a2. Regresa a la lista de servicios o al menú principal.**

**Escenario de éxito:**

**El administrador pudo modificar el servicio con éxito. Los nuevos datos (precio, nombre, etc.) se reflejan inmediatamente en el catálogo y en las opciones para los clientes.**

**Escenario de fracaso:**

**El administrador no pudo modificar el servicio debido a datos inválidos o cancelación de la operación y el servicio permanece sin cambios en el catálogo.**

