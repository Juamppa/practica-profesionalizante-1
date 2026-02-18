**Caso de Uso: Registrar nuevo servicio**

**Actor primario: Administrador**

**Precondiciones:**

* **El Administrador está autenticado en el sistema El Administrador tiene permisos para gestionar el catálogo de servicios.**

**Camino básico:**

1. **El usuario selecciona la opción "Agregar servicio" desde el panel de administración.**  
2. **El sistema muestra el formulario para ingresar los datos del servicio.**  
3. **El usuario completa los campos obligatorios: nombre del servicio y precio.**  
4. **El sistema valida los datos ingresados (campos completos, precio \> 0, nombre no duplicado, etc.).**  
5. **El usuario presiona "Aceptar" para confirmar el registro.**  
6. **El sistema registra el servicio en el catálogo y muestra el mensaje: "Servicio registrado correctamente".**

**Postcondiciones:**

* **El nuevo servicio está disponible en el catálogo del sistema.**  
* **Puede ser seleccionado por clientes al solicitar turnos.**

**Caminos alternativos:**

**4a. Datos inválidos o incompletos**  
**4a1. El sistema muestra mensajes de error específicos junto a los campos problemáticos (ej. "Precio debe ser mayor a 0", "Nombre obligatorio").**  
**4a2. El sistema mantiene el formulario abierto.**

**4a3. El Administrador corrige los datos y vuelve a presionar "Aceptar" (regresa al paso 5).**

**4b. Nombre de servicio ya existente**

**4b1. El sistema muestra un mensaje: "Ya existe un servicio con ese nombre".**

**4b2. El sistema mantiene el formulario abierto.**  
**4b3. El Administrador modifica el nombre y vuelve a confirmar.**

**Escenario de éxito:**

**El administrador pudo registrar el nuevo servicio con éxito y este aparece inmediatamente en el catálogo disponible para los clientes.**

**Escenario de fracaso:**

**El administrador no pudo registrar el servicio debido a datos inválidos o duplicados y el servicio no se agrega al catálogo.**

