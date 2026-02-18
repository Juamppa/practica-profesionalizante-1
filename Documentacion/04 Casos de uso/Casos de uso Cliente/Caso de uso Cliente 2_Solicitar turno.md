**Caso de Uso: Solicitar turno**

**Actor primario: Cliente**

**Precondiciones:**

* **El Cliente está identificado en el sistema (ver caso de uso "Identificarse como cliente").**  
* **Existen servicios, profesionales y horarios disponibles en el catálogo del sistema.**

**Camino básico:**

1. **El usuario selecciona la opción "Solicitar turno" desde el panel de cliente.**  
2. **El sistema muestra la lista de servicios disponibles.**  
3. **El usuario selecciona uno o más servicios.**  
4. **El sistema muestra las fechas y horas disponibles según los servicios y profesionales.**  
5. **El usuario selecciona una fecha y hora.**  
6. **El sistema muestra los profesionales disponibles para esa fecha/hora y servicios seleccionados.**  
7. **El usuario selecciona un profesional.**  
8. **El sistema envía un código de verificación único por WhatsApp al teléfono del cliente y reserva provisionalmente el turno.**  
9. **El usuario ingresa el código recibido en el formulario del sistema.**  
10. **El sistema valida el código ingresado.**  
11. **El usuario confirma la reserva.**  
12. **El sistema confirma la reserva definitiva y muestra el mensaje: "Turno agendado correctamente. Recibirás una confirmación por WhatsApp".**

**Postcondiciones:**

* **El turno queda guardado en la base de datos con estado "Confirmado".**  
* **El horario seleccionado del profesional queda bloqueado para otros turnos.**  
* **El cliente recibe una confirmación por WhatsApp.**  
* **El turno aparece en el historial o lista del cliente.**

**Caminos alternativos:**

**3a. No hay servicios disponibles en el catálogo**  
**3a1. El sistema muestra el mensaje: "No hay servicios disponibles en este momento".**  
**3a2. El sistema regresa al menú principal o permite al Cliente esperar/actualizar la lista.**

**3a3. El Cliente puede cancelar la solicitud o volver al menú principal.**

**5a. No hay fechas/horas disponibles para los servicios seleccionados**  
**5a1. El sistema muestra el mensaje: "No hay horarios disponibles para los servicios elegidos".**

**5a2. El sistema permite al Cliente seleccionar otros servicios o cambiar filtros (regresa al paso 3 o 5).**

**7a. No hay profesionales disponibles para la fecha/hora seleccionada.**  
**7a1. El sistema muestra el mensaje: "No hay profesionales disponibles en ese horario para los servicios elegidos".**

**7a2. El sistema permite al Cliente cambiar fecha/hora o servicios (regresa al paso 5 o 3).**

**9a. Código ingresado incorrecto**  
**9a1. El sistema muestra el mensaje: "Código incorrecto".**  
**9a2. El sistema permite reingresar el código.**  
**9b. Código expirado luego de 1 minuto desde envío.**  
**9b1. El sistema muestra el mensaje: "El código ha expirado".**

**9b2. El sistema ofrece reenviar un nuevo código (regresa al paso 8\) o cancelar la operación.**

**10a. Código inválido o error en validación**  
**10a1. El sistema muestra un mensaje: "El código no es válido o ha ocurrido un error".**

**10a2. El Cliente puede reintentar ingresar código o cancelar (regresa al paso 9 o termina).**

**11a. El Cliente cancela la confirmación final.**  
**11a1. El sistema cancela la reserva provisional.**  
**11a2. El sistema muestra el mensaje: "Reserva cancelada".**

**11a3. Regresa al menú principal o a la lista de turnos.**

**Escenario de éxito:**

**El cliente completa la selección de servicios, fecha/hora y profesional, ingresa correctamente el código de verificación recibido por WhatsApp, confirma la reserva y recibe el mensaje de éxito. El turno queda agendado y confirmado en el sistema.**

**Escenario de fracaso:**

**El cliente no logra completar la solicitud debido a falta de disponibilidad (servicios, horarios, profesionales), código incorrecto/expirado o cancelación, y el turno no se registra ni se confirma.**

