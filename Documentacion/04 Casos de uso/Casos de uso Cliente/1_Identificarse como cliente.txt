## Caso de Uso: Identificarse como cliente

**Actor primario:** Cliente

**Camino básico:**

1. **El usuario** ingresa sus datos personales (nombre, apellido, teléfono y correo electrónico) y los envía.
2. **El sistema** recibe los datos y verifica que sean válidos.

**Postcondiciones:**
- El perfil del cliente está reconocido o creado en la base de datos.
- El cliente accede a la interfaz principal y puede realizar las operaciones disponibles.

**Caminos alternativos:**

**2a. Datos inválidos o incompletos.**

2a1. **El sistema** muestra un mensaje indicando que los datos ingresados son incorrectos o que faltan campos obligatorios.

2a2. **El usuario** corrige los datos y los vuelve a enviar.

2a3. **El sistema** recibe nuevamente los datos y verifica que sean válidos.

**2b. Datos inconsistentes con un perfil existente.**

2b1. **El sistema** informa que los datos ingresados no coinciden con el perfil registrado.

2b2. **El usuario** corrige sus datos y los vuelve a enviar.

2b3. **El sistema** recibe nuevamente los datos y verifica que sean válidos.

**Escenario de éxito:**

El cliente ingresa sus datos correctamente y los envía. El sistema verifica que sean válidos y permite continuar con el proceso de identificación.

**Escenario de fracaso:**

El cliente no logra identificarse debido a datos inválidos o inconsistentes, por lo que no puede acceder a la interfaz principal.