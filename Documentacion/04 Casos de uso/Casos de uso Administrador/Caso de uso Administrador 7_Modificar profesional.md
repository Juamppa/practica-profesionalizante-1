**Caso de Uso: Modificar profesional**

**Actor primario: Administrador**

**Precondiciones:**

* **El Administrador está autenticado en el sistema.**  
* **El Administrador tiene permisos para gestionar los profesionales.**  
* **Existe al menos un profesional registrado en el sistema.**

**Camino básico:**

1. **El usuario selecciona la opción "Modificar profesional" desde el panel de administración.**  
2. **El sistema muestra la lista de profesionales registrados.**  
3. **El usuario selecciona el profesional que desea modificar.**  
4. **El sistema muestra el formulario con los datos actuales del profesional precargados.**  
5. **El usuario modifica los campos necesarios (por ejemplo, disponibilidad, nombre, apellido, etc.).**  
6. **El sistema valida los datos modificados (campos obligatorios completos, formatos correctos, etc.).**  
7. **El usuario presiona "Aceptar" para confirmar los cambios.**  
8. **El sistema actualiza el profesional en el sistema y muestra el mensaje: "Profesional modificado correctamente".**

**Postcondiciones:**

* **El profesional queda actualizado con los nuevos datos.**  
* **Los cambios se reflejan inmediatamente en las opciones disponibles para asignar turnos.**

**Caminos alternativos:**

**3a. Ningún profesional seleccionado**  
**3a1. El sistema muestra el mensaje: "Debe seleccionar al menos un profesional para modificar".**  
**3a2. El sistema mantiene la lista visible.**

**3a3. El Administrador selecciona un profesional y continúa.**

**5a/6a. Datos modificados inválidos o incompletos.**  
**6a1. El sistema muestra mensajes de error específicos junto a los campos problemáticos (ej. "Disponibilidad no válida", "Nombre obligatorio").**  
**6a2. El sistema mantiene el formulario abierto con los cambios parciales.**

**6a3. El Administrador corrige los datos y vuelve a confirmar.**

**7a. El Administrador cancela los cambios.**  
**7a1. El sistema cierra el formulario sin guardar nada.**

**7a2. Regresa a la lista de profesionales o al menú principal.**

**Escenario de éxito:**

**El administrador pudo modificar el profesional con éxito. Los nuevos datos (disponibilidad, nombre, etc.) se reflejan inmediatamente en el sistema y en las opciones para asignar turnos.**

**Escenario de fracaso:**

**El administrador no pudo modificar el profesional debido a datos inválidos o cancelación de la operación, y el profesional permanece sin cambios en el sistema.**

