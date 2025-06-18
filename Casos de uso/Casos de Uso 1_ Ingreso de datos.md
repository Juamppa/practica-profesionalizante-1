# Caso de Uso

**Caso de Uso:** Ingreso de datos

**Actores:**   
\-Usuario (primario)

**Pre-condiciones:**   
\-El usuario debe contar con acceso a internet.

**Camino básico:** 

1. El usuario ingresa a la página.   
2. La página pide al usuario ingresar nombre, apellido, teléfono y mail.  
3. El usuario debe ingresar los datos solicitados.  
4. La página valida los datos.  
5. El usuario accede a la interfaz principal. 

**Caminos alternativos:**  
1.a. La página está caída  
1.a.1. La página muestra el mensaje “No se puede acceder a este sitio web”.  
4.a. Los datos ingresados son incorrectos o no válidos.  
4.a.1 El sistema muestra el mensaje “mail invalido”. Vuelve al paso 3\.  
4.a.2 El sistema muestra el mensaje “teléfono inexistente”: Vuelve al paso 3\.  
   
**Escenario de éxito:**   
El usuario ingresa a la interfaz principal.

**Escenario de fracaso:**  
El usuario ingresa mal sus datos y no puede ingresar a la interfaz principal.  
La página está fuera de servicio.

**Post-condiciones:**
1. El usuario debe poder ingresar a la solicitud de turnos.
2. El sistema almacena los datos del usurio ingresados en la base de datos.