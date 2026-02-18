**Caso de Uso: Autenticar como Administrador**

**Actor primario: Administrador**

**Precondiciones:**

* **El administrador tiene un número de teléfono registrado en el sistema.**  
* **El administrador tiene acceso a WhatsApp en el teléfono registrado.**  
* **Existe conexión a internet.**

**Camino básico:**

1. **El usuario accede a la página principal del sistema.**  
2. **El sistema muestra las opciones de inicio de sesión: "Cliente" o "Administrador".**  
3. **El usuario selecciona la opción "Administrador".**  
4. **El sistema solicita el número de teléfono registrado.**  
5. **El usuario ingresa su número de teléfono.**  
6. **El sistema valida que el número esté registrado y envía un código de verificación único vía WhatsApp al número ingresado.**  
7. **El usuario recibe el código de verificación.**  
8. **El sistema solicita el código de verificación recibido.**  
9. **El usuario ingresa el código recibido.**  
10. **El sistema valida el código.**  
11. **El sistema otorga acceso al panel de administración.**  
    

**Caminos alternativos:**

**5a. Número de teléfono no registrado o incorrecto.**  
**5a1. El sistema muestra el mensaje: "El número ingresado no está registrado como administrador".**

**5a2. Permite reintentar (volver al paso 4\) o regresar a la pantalla inicial.**

**9a. Código ingresado incorrecto.**  
**9a1. El sistema muestra el mensaje: "Código incorrecto".**  
**9a2. Permite reintentar.**

**Escenario de éxito: El Administrador accede correctamente al panel de administración.**

**Escenario de fracaso: El Administrador no logra autenticarse después de varios intentos o por error técnico.**

