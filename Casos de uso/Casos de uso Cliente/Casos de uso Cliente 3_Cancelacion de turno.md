# Caso de Uso

**Caso de Uso:** Cancelación de turno

**Actores:**   
\-Cliente (primario)

**Camino básico:** 


1. El usuario ingresa a la página web.
2. La página muestra los botones de opción de inicio de sesión como cliente o como administrador.
3. El usuario debe ingresa al apartado cliente.
4. La página solicita al cliente el nombre, apellido, teléfono y mail.
5. El cliente ingresa sus datos.
6. La página valida los datos.
7. El cliente accede a la interfaz principal del cliente.
8. La página muestra en pantalla la opción "Cancelar turno".
9. El cliente selecciona su turno a cancelar.
10. La página cancela el turno con éxito.
     

**Caminos alternativos:** 

**5.a.** Los datos ingresados son incorrectos o no válidos.

**5.a.1.** La página muestra el mensaje “mail invalido”. Vuelve al paso 3.

**5.a.2.** La página muestra el mensaje “teléfono inexistente”: Vuelve al paso 3.

**9.a.** El cliente selecciona un turno fuera del tiempo estipulado para su cancelación.  

**9.a.1.** La página muestra en pantalla el mensaje “Su turno no puede ser cancelado con menos de 24 horas de antelación”.

**Escenario de éxito:**   
Se pudo cancelar un turno exitosamente.

**Escenario de fracaso:**  
El cliente no puede cancelar su turno.

**Post-condiciones:**  
El turno es eliminado de la agenda de turnos.  
