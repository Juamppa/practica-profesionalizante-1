### **Caso de Uso: Cancelar turno**

**Caso de Uso: Cancelar turno**

**Actor primario: Cliente**

**Precondiciones:**

* **El Cliente está identificado en el sistema.**  
* **El Cliente tiene al menos un turno agendado en el sistema.**  
* **El turno a cancelar está en estado activo.**

**Camino básico:**

1. **El usuario selecciona la opción "Mis turnos" o "Cancelar turno" desde el panel de cliente.**  
2. **El sistema muestra la lista de turnos agendados del cliente con fecha, hora, profesional, servicios.**  
3. **El usuario selecciona el turno que desea cancelar.**  
4. **El sistema muestra los detalles del turno y un mensaje de confirmación "¿Está seguro de cancelar este turno?".**  
5. **El usuario confirma la cancelación presionando "Cancelar" o "Aceptar".**  
6. **El sistema verifica que el turno cumpla con la regla de anticipación y elimina el turno mostrando el mensaje  "Turno cancelado correctamente".**

**Postcondiciones:**

* **El turno es eliminado de la base de datos y de la agenda del profesional.**  
* **El horario del profesional queda liberado para otros clientes.**  
* **El turno desaparece de la lista de turnos del cliente.**  
* **El cliente recibe notificación por WhatsApp.**

**Caminos alternativos:**

**3a. No hay turnos agendados para el cliente**

**3a1. El sistema muestra un mensaje: "No tienes turnos agendados en este momento".**

**3a2. El sistema regresa al menú principal.**

**3a3. El Cliente puede volver a la interfaz principal.**

**3b. El Cliente no selecciona ningún turno.**

**3b1. El sistema muestra un mensaje: "Debe seleccionar un turno para cancelar".**

**3b2. El sistema mantiene la lista visible.**

**3b3. El Cliente selecciona un turno y continúa (regresa al paso 5).**

**5a. El Cliente cancela la operación de cancelación.**

**5a1. El sistema cierra el diálogo de confirmación sin eliminar nada.**

**6a. El turno no cumple la regla de 24 horas de anticipación.**

**6a1. El sistema muestra el mensaje: "Su turno no puede ser cancelado con menos de 24 horas de antelación".**

**6a2. El sistema mantiene el turno intacto.**

**6a3. El Cliente puede regresar a la lista o al menú principal.**

**6b. El turno ya pasó o está en estado no cancelable.**

**6b1. El sistema muestra un mensaje: "Este turno ya pasó o no puede ser cancelado".**

**6b2. El sistema no elimina nada.**

**6b3. Regresa a la lista de turnos.**

**Escenario de éxito:**

**El cliente puede cancelar el turno correctamente.**

**Escenario de fracaso:**

**El cliente no logra cancelar el turno seleccionado.**

