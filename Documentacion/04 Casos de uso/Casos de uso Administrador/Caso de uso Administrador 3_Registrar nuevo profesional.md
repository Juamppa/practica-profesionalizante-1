**Caso de Uso: Registrar nuevo profesional**

**Actor primario: Administrador**

**Precondiciones:**

* **El Administrador está autenticado en el sistema.**  
* **El Administrador tiene permisos para gestionar los profesionales.**

**Camino básico:**

1. **El usuario selecciona la opción "Agregar profesional" desde el panel de administración.**  
2. **El sistema muestra el formulario para ingresar los datos del profesional.**  
3. **El usuario completa los campos obligatorios: nombre, apellido y disponibilidad (horarios o días disponibles).**  
4. **El sistema valida los datos ingresados (campos completos, formatos correctos, etc.).**  
5. **El usuario presiona "Aceptar" para confirmar el registro.**  
6. **El sistema registra el nuevo profesional en el sistema y muestra el mensaje: "Profesional registrado correctamente".**

**Postcondiciones:**

* **El nuevo profesional está disponible en el sistema.**  
* **Puede ser asignado a turnos y aparecer en las opciones para los clientes.**

**Caminos alternativos:**

**4a. Datos inválidos o incompletos**  
**4a1. El sistema muestra mensajes de error específicos junto a los campos problemáticos (ej. "Nombre obligatorio", "Apellido obligatorio").**  
**4a2. El sistema mantiene el formulario abierto.**

**4a3. El Administrador corrige los datos y vuelve a presionar "Aceptar".**

**4b. Profesional con nombre/apellido ya existente.**

**4b1. El sistema muestra el mensaje: "Ya existe un profesional con ese nombre y apellido".**  
**4b2. El sistema mantiene el formulario abierto.**

**4b3. El Administrador modifica los datos o los cancela.**

**Escenario de éxito:**

**El administrador pudo registrar el nuevo profesional con éxito y este aparece inmediatamente en la lista de profesionales disponibles para asignar turnos.**

**Escenario de fracaso:**

**El administrador no pudo registrar el profesional debido a datos inválidos o duplicados y el profesional no se agrega al sistema.**

