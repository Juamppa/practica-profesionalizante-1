## Caso de Uso: Solicitar turno

**Actor primario:** Cliente

**Precondiciones:**
- Existen servicios, profesionales y horarios disponibles en el sistema.

**Camino básico:**

1. **El usuario** selecciona los servicios, el profesional, la fecha y el horario deseados, y envía la solicitud.
2. **El sistema** recibe la solicitud y verifica que los datos sean válidos y que el horario seleccionado esté disponible.
3. **El usuario** confirma la solicitud del turno.
4. **El sistema** registra el turno en la base de datos con estado "Confirmado", bloquea el horario seleccionado del profesional y envía un correo electrónico al cliente informando la confirmación del turno.

**Postcondiciones:**
- El turno queda guardado en la base de datos con estado "Confirmado".
- El horario seleccionado del profesional queda bloqueado para otros turnos.
- El cliente recibe un correo electrónico de confirmación.
- El turno aparece en el historial o lista de turnos del cliente.

**Caminos alternativos:**

**2a. Datos incompletos o inválidos.**

2a1. **El sistema** informa que faltan datos obligatorios o que la información ingresada no es válida.

2a2. **El usuario** corrige los datos y vuelve a enviar la solicitud.

2a3. **El sistema** recibe nuevamente la solicitud y verifica los datos ingresados.

**2b. El horario seleccionado ya no está disponible.**

2b1. **El sistema** informa que el horario seleccionado no se encuentra disponible.

2b2. **El usuario** selecciona otro horario y vuelve a enviar la solicitud.

2b3. **El sistema** verifica nuevamente la disponibilidad del horario seleccionado.

**2c. No existen servicios disponibles.**

2c1. **El sistema** informa que no hay servicios disponibles para realizar la reserva.

**2d. No existen profesionales disponibles para la fecha y horario seleccionados.**

2d1. **El sistema** informa que no hay profesionales disponibles para el horario solicitado.

**Escenario de éxito:**

El cliente selecciona los servicios, el profesional, la fecha y el horario deseados, envía la solicitud y el sistema verifica la disponibilidad. El turno queda registrado y confirmado, y el cliente recibe un correo electrónico de confirmación.

**Escenario de fracaso:**

El cliente no logra completar la solicitud debido a datos inválidos, falta de disponibilidad de servicios, profesionales u horarios. El turno no queda registrado ni confirmado.