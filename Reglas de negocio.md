# **REGLAS DE NEGOCIO**

Hechos
* Un profesional no puede tener dos turnos asignados al mismo tiempo.   
*  La barbería solo atiende en horario laboral (por ejemplo, de martes a sábado de 10:00 a 20:00 hs).
*  La barberia no puede confirmar turnos fuera del horario laboral.
*  El cliente siempre es atendido por un barbero profesional.
*  Cada servicio tiene un precio asignado.
    
Restricciones  
*  Los horarios disponibles dependen de la agenda de cada profesional.
*  No aceptar turnos de clientes deudores.
*  Los turnos solicitados despues de las 20:00, seran confirmados a primera hora del siguiente día habil. 
 
Acciones disparadoras  
* La confirmación por WhatsApp debe enviarse como máximo 1 minuto después de hecha la reserva.  
* Cuando un cliente supera 3 cortes consecutivos en un mes se le aplica un descuento del 10% en su proximo corte.
    
Cálculo  
* El valor del servicio se calcula en base al o los servicios que solicite el cliente.

Inferencia
* Si no se abona el pago del servicio, el cliente queda registrado en el sistema como deudor.
* Si el profesional debe cancelar el turno por algun motivo, el turno sera reprogramado para la fecha mas cercana a su turno anterior. 