## Caso de Uso: Registrar nuevo profesional

**Actor primario:** Administrador

**Precondiciones:**

- El Administrador está autenticado en el sistema.
- El Administrador tiene permisos para gestionar los profesionales.

**Camino básico:**

1. **El usuario** ingresa el nombre, apellido y disponibilidad del profesional.
2. **El sistema** valida que los campos obligatorios estén completos y que los datos ingresados tengan formatos correctos.
3. **El usuario** confirma el registro del nuevo profesional.
4. **El sistema** registra al profesional y confirma que el registro se realizó correctamente.

**Postcondiciones:**

- El nuevo profesional queda registrado en el sistema.
- El profesional queda disponible para ser asignado a turnos y seleccionado por los clientes.

**Caminos alternativos:**

**4a. Datos inválidos o incompletos**

4a1. **El sistema** informa que los datos ingresados son inválidos o están incompletos.

4a2. **El usuario** corrige los datos solicitados.

4a3. **El sistema** valida nuevamente los datos ingresados.

**4b. Profesional con nombre y apellido ya existentes**

4b1. **El sistema** informa que ya existe un profesional registrado con ese nombre y apellido.

4b2. **El usuario** modifica los datos del profesional.

4b3. **El sistema** valida nuevamente los datos ingresados y continúa con el proceso de registro si son correctos.

**Escenario de éxito:**

El administrador registra correctamente al nuevo profesional y el sistema lo incorpora a la lista de profesionales disponibles para asignar turnos.

**Escenario de fracaso:**

El sistema no registra al profesional debido a datos inválidos, incompletos o a la existencia de otro profesional con el mismo nombre y apellido.