# Caso de Uso

**Caso de Uso:** Solicitud de turno

**Actores:**   
\-Usuario (primario)

**Camino básico:** 

1. El sistema muestra en pantalla los servicios disponibles.  
2. El usuario selecciona uno de los servicios.  
3. El sistema muestra en pantalla fecha y hora disponibles.  
4. El usuario selecciona la fecha y hora.  
5. El sistema muestra en pantalla los profesionales disponibles.  
6. El usuario selecciona uno de los profesionales.
7. El sistema envía un mensaje de confirmación al teléfono del usuario.
   

**Caminos alternativos:**  
6.a No hay profesionales disponibles para la fecha y horario seleccionados. Vuelve al paso 5.

**Escenario de éxito:**   
El usuario puede agendar el servicio el día seleccionado.

**Escenario de fracaso:**  
El usuario no puede agendar el día por falta de disponibilidad de los profesionales.  

**Post-condiciones:**
1. El usuario debe poder reservar el turno.
2. El turno debe quedar guardado en la base de datos.