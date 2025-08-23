# Caso de Uso

**Caso de Uso:** Inicio de sesión como administrador

**Actores:**   
\-Administrador (primario)

**Pre-condiciones:**
-Debe haber un número de teléfono previamente registrado en el código.

**Camino básico:** 

1. El usuario ingresa a la página web.
2. La página muestra los botones de opcion de inicio de sesion como cliente o como administrador.
3. El usuario ingresa al apartado de administrador.
4. La página solicita al usuario el número de teléfono.
5. El usuario carga su número de teléfono.
6. La página valida que sea el número cargado previamente por código y envía un mensaje de whatsapp al usuario con un código de verificación que solicita para iniciar sesión.
7. El usuario ingresa el código recibido por whatsapp en la página.
8. La página accede a la interfaz principal del administrador.
    

**Caminos alternativos:** 

**5.a.** El número de teléfono ingresado no es correcto.

**5.a.1.** La página muestra en pantalla el mensaje “El número de teléfono ingresado no es correcto”.

**7.a.** El código ingresado no es correcto.

**7.a.1.** La página muestra en pantalla el mensaje “El código ingresado no es correcto”.

**Escenario de éxito:**   
Se pudo acceder a la interfaz de administrador exitosamente.

**Escenario de fracaso:**  
El usuario no puede acceder a la interfaz de administrador.

