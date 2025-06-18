# Caso de Uso

**Caso de Uso:** Cancelación de turno

**Actores:**   
\-Usuario (primario)

**Pre-condiciones:**  
 El turno puede ser cancelado por la página únicamente 24 horas antes.

**Camino básico:** 

1. El usuario ingresa por la página a la agenda de turnos que quiere cancelar.  
2. El sistema muestra en pantalla la agenda de turnos con la opción “Cancelar turno”.  
3. El usuario selecciona su turno y lo cancela.  
4. El sistema muestra en pantalla el mensaje “Su turno ha sido cancelado”.  
     
   

**Caminos alternativos:**  
**3.a.** El usuario selecciona su turno fuera del tiempo estipulado para su cancelación.  
**3.a.1** El sistema muestra en pantalla el mensaje “Su turno no puede ser cancelado con menos de 24 horas de antelación”.

**Escenario de éxito:**   
Se puede cancelar el turno exitosamente.

**Escenario de fracaso:**  
El usuario no puede cancelar su turno exitosamente.

**Post-condiciones:**  
El turno es eliminado de la agenda de turnos.  
