## Caso de Uso: Autenticar como Administrador

**Actor primario:** Administrador

**Precondiciones:**
- El administrador tiene una cuenta de Gmail registrada previamente en el sistema.

**Camino básico:**

1. **El usuario** ingresa su Gmail registrado y envía sus datos.
2. **El sistema** verifica que el Gmail corresponda a una cuenta de administrador y permite el acceso

**Postcondiciones:**
- El administrador accede correctamente al panel de administración.
- El sistema reconoce al usuario como administrador.

**Caminos alternativos:**

**2a. Gmail no registrado como administrador.**

2a1. **El sistema** informa que el Gmail ingresado no corresponde a una cuenta de administrador.

2a2. **El usuario** corrige sus datos y vuelve a enviarlos.

2a3. **El sistema** verifica nuevamente el Gmail ingresado.

**Escenario de éxito:**

El administrador ingresa su Gmail registrado, el sistema lo reconoce como administrador y le permite acceder al panel de administración.

**Escenario de fracaso:**

El administrador no logra acceder al panel de administración debido a que el Gmail ingresado no está registrado como administrador o se produce un error técnico.