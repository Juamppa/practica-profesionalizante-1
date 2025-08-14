# Caso de Uso

**Caso de Uso:** Cancelación de turno

**Actores:**   
\-Usuario (primario)

**Camino básico:** 

1. El usuario ingresa a la página.
2. La página debe mostrar al usuario los campos para ingresar nombre, apellido, teléfono y mail.
3. El usuario debe ingresar nombre, apellido, teléfono y mail.
4. La página valida los datos.
5. El usuario accede a la interfaz principal.
6. El sistema muestra en pantalla la agenda de turnos con la opción “Cancelar turno”. 
7. El usuario selecciona su turno y lo cancela.  
8. El sistema muestra en pantalla el mensaje “Su turno ha sido cancelado”.  
     

**Caminos alternativos:** 
**4.a.** Los datos ingresados son incorrectos o no válidos.
**4.a.1.** El sistema muestra el mensaje “mail invalido”. Vuelve al paso 3.
**4.a.2.** El sistema muestra el mensaje “teléfono inexistente”: Vuelve al paso 3.
**7.a.** El usuario selecciona su turno fuera del tiempo estipulado para su cancelación.  
**7.a.1** El sistema muestra en pantalla el mensaje “Su turno no puede ser cancelado con menos de 24 horas de antelación”.

**Escenario de éxito:**   
Se puedo cancelar el turno exitosamente.

**Escenario de fracaso:**  
El usuario no puede cancelar su turno.

**Post-condiciones:**  
El turno es eliminado de la agenda de turnos.  
