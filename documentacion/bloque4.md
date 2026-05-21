# Bloque 4 - Diseño de casos de prueba
## Tarea 4: diseño de casos de prueba
   ID,Funcionalidad,Objetivo,Datos de entrada,Resultado esperado,Tipo de caso
CP-001,Validación de edad,Comprobar edad inferior a 16,int edad = 15;,"""El usuario debe tener por lo menos 16 años""",Caso inválido
CP-002,Validación de edad,Comprobar edad igual a 16,int edad = 16;,"""Registro válido""",Caso normal
CP-003,Validación de edad,Comprobar edad superior a 16,int edad = 19;,"""Registro válido""",Caso normal
CP-004,Validación tarjeta activa,Comprobar descuento a usuarios con tarjeta,boolean tarjetaActiva = true;,precio = 0;,Caso normal
CP-005,Validación tarjeta activa,Aplicación de tasa a usuarios sin tarjeta,boolean tarjetaActiva = false;,this.precio += 2;,Caso normal
CP-006,Validación edad,"Rangos fuera de límites (-12, 121)",int edad = -12;int edad = 121;,"I: ""Número inválido""II: ""Número inválido""",Caso inválido
CP-007,Clase de equivalencia,"Valores inválidos (rango >120, <16, negativos, 0)","121, 15, -1, 0","I: ""Número inválido""II: ""El usuario debe ser mayor de 16""III/IV: ""Número inválido""",Clase equiv. inválida
CP-008,Clase de equivalencia,Valores válidos (dentro del rango permitido),"16, 120, 20","""Registro válido""",Clase equiv. válida
### Explicación detallada de un caso de prueba
   Campo,Respuesta
Identificador,CP-002
Funcionalidad,Validación de edad
Objetivo,Verificar que se validan usuarios con edad igual a 16
Datos de entrada,int edad = 16;
Resultado esperado,“Registro válido!”
Tipo de caso,Valor límite
Motivo por el que se ha elegido,Porque es un punto crítico donde cambia la lógica de la aplicación (la frontera entre no permitido y permitido); es un punto de alta probabilidad de error en pruebas de caja blanca y negra.
### Respuestas razonadas
   • ¿Qué casos corresponden a valores límite?
En CP007

• ¿Qué casos corresponden a datos inválidos?

CP001 - CP006
• ¿Qué casos comprueban el acceso gratuito?

CP004

• ¿Qué casos comprueban el acceso con pago?

CP005
• ¿Qué casos comprueban que el acceso debe rechazarse?

CP001 CP002 CP007

• ¿Por qué no sería suficiente probar solo con una persona de 18 años y tarjeta activa?

Porque dentro de todo el escopo de las posibles entradas de usuario, 18 y tarjeta activa no abarcan virtualmente nada: sería como si la vacuna del covid la hubieran probado en mi primo y así decidido que era seguro y funcional para cualquier persona del planeta

