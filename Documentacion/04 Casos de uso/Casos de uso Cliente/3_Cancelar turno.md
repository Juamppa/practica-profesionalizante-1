## Caso de Uso: Cancelar turno

**Actor primario:** Cliente

**Precondiciones:**
- El cliente está identificado en el sistema.
- El cliente tiene al menos un turno agendado en el sistema.
- El turno a cancelar está en estado activo.

**Camino básico:**

1. **El usuario** solicita consultar sus turnos agendados.
2. **El sistema** muestra los turnos registrados del cliente con fecha, hora, profesional y servicios.
3. **El usuario** selecciona el turno que desea cancelar y solicita su cancelación.
4. **El sistema** verifica que el turno cumpla con la anticipación mínima de 24 horas, lo elimina de la agenda, libera el horario del profesional y confirma la cancelación.

**Postcondiciones:**
- El turno es eliminado de la agenda del profesional.
- El horario del profesional queda liberado para otros clientes.
- El turno deja de figurar entre los turnos activos del cliente.

**Caminos alternativos:**

**2a. No hay turnos agendados para el cliente.**

2a1. **El sistema** informa que el cliente no tiene turnos agendados.

**4a. El turno no cumple con la regla de 24 horas de anticipación.**

4a1. **El sistema** informa que el turno no puede ser cancelado con menos de 24 horas de antelación.

**4b. El turno ya pasó o se encuentra en un estado no cancelable.**

4b1. **El sistema** informa que el turno seleccionado ya pasó o no puede ser cancelado.

**Escenario de éxito:**

El cliente selecciona un turno que cumple con las condiciones de cancelación y solicita su cancelación. El sistema elimina el turno de la agenda y libera el horario del profesional.

**Escenario de fracaso:**

El cliente no logra cancelar el turno debido a que no cumple con la anticipación mínima de 24 horas, el turno ya pasó o se encuentra en un estado no cancelable.