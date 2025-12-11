# **REGLAS DE NEGOCIO**

Hechos
* Un profesional no puede tener dos turnos asignados al mismo tiempo.   
*  El cliente siempre es atendido por un barbero profesional.
*  Cada servicio tiene un precio asignado.
    
Restricciones  
*  Los horarios disponibles dependen de la agenda de cada profesional. 
*  Los turnos pueden ser cancelados unicamente con 24 horas o más de anticipación.
 
Acciones disparadoras  
* La confirmación por WhatsApp debe enviarse como máximo 1 minuto después de hecha la reserva.  
 
    
Cálculo  
* El valor del servicio se calcula en base al o los servicios que solicite el cliente.

Inferencia
* Si no se abona el pago del servicio, el cliente queda registrado en el sistema como deudor.
 