# Caso de Uso

**Caso de Uso:** Solicitud de turno

**Actores:**   
\-Cliente (primario)

**Camino básico:** 

1. La página muestra en pantalla los servicios disponibles.  
2. El cliente selecciona uno de los servicios.  
3. La página muestra en pantalla fecha y hora disponibles.  
4. El cliente selecciona la fecha y hora.  
5. La página muestra en pantalla los profesionales disponibles.  
6. El cliente selecciona uno de los profesionales.
7. La página envía un codigo de verificación único al cliente a través de whatsapp.
   


**Escenario de éxito:**   
El cliente puede agendar el servicio el día seleccionado.

**Escenario de fracaso:**  
El cliente no puede agendar su turno.  

**Post-condiciones:**
El turno debe quedar guardado en la base de datos.