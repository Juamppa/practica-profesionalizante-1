**Caso de Uso: Identificarse como cliente**

**Actor primario: Cliente**

**Precondiciones:**

* **El cliente cuenta con acceso a internet.**  
* **El cliente accede a la página web del sistema.**

**Camino básico:**

1. **El usuario accede a la página principal del sistema.**  
2. **El sistema muestra las opciones: "Iniciar como Cliente" o "Iniciar como Administrador".**  
3. **El usuario selecciona "Iniciar como Cliente".**  
4. **El sistema muestra el formulario para ingresar datos personales: nombre, apellido, teléfono y email.**  
5. **El usuario completa y envía sus datos.**  
6. **El sistema valida el formato de los datos (email válido, teléfono correcto, campos obligatorios completos).**  
7. **El usuario presiona "Continuar" o "Aceptar" después de la validación.**  
8. **El sistema reconoce o crea el perfil del cliente y le otorga acceso a la interfaz principal del cliente.**

**Postcondiciones:**

* **El perfil del cliente está reconocido o creado en la base de datos.**  
* **El cliente está en la interfaz principal y puede realizar acciones (ver turnos, solicitar, cancelar, etc.).**

**Caminos alternativos:**

**6a. Datos con formato inválido.**  
**6a1. El sistema muestra mensajes de error específicos junto a los campos (ej. "Email inválido", "Teléfono debe tener 10 dígitos", "Campo obligatorio faltante").**  
**6a2. El sistema mantiene el formulario abierto con los datos ingresados.**

**6a3. El Cliente corrige y vuelve a enviar.**

**6b. Datos inconsistentes (ej. mismo teléfono pero nombre/apellido diferente)**  
**6b1. El sistema muestra el mensaje: "Los datos ingresados no coinciden con un perfil existente. Verifique la información o use datos diferentes".**

**6b2. El Cliente corrige los datos o cancela.**

**Escenario de éxito:**

**El cliente ingresa sus datos correctamente, el sistema los reconoce o crea el perfil, y accede a la interfaz principal del cliente.**

**Escenario de fracaso:**

**El cliente no logra identificarse debido a datos inválidos o inconsistentes, y no accede a la interfaz principal.**

