# Caso de Uso

**Caso de Uso:** Identificación de usuario

**Actores:**   
\-Cliente (primario)

**Pre-condiciones:**   
\-El usuario debe contar con acceso a internet.

**Camino básico:** 

1. El usuario ingresa a la página web.
2. La página muestra los botones de opción de inicio de sesión como cliente o como administrador.
3. El usuario debe ingresa al apartado cliente.
4. La página solicita al cliente el nombre, apellido, teléfono y mail.
5. El cliente ingresa sus datos.
6. La página valida los datos.
7. El cliente accede a la interfaz principal del cliente.

**Caminos alternativos:**

5.a. Los datos ingresados son incorrectos o no válidos.  

5.a.1. La página muestra el mensaje “mail invalido”. Vuelve al paso 3\.  

5.a.2. La página muestra el mensaje “teléfono inexistente”: Vuelve al paso 3\.  
   
**Escenario de éxito:**   
El cliente ingresa a la interfaz principal del cliente.

**Escenario de fracaso:**  
El cliente ingresa mal sus datos y no puede ingresar a la interfaz principal del cliente.  

**Post-condiciones:**

La página almacena los datos del usurio ingresados en la base de datos.
