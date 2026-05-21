# Bloque 3 - Planificación de pruebas
## Tarea 3: planificación inicial de pruebas
 
| Funcionalidad | Qué se debe comprobar | Datos que conviene probar |
| --- | --- | --- |
| Validación de edad mínima | que la edad es igual o superior a 12 | 11, 12, 13 |
| Validación de edad máxima | que la edad es igual o inferior a 18 | 17, 18, 19 |
| Comprobación de autorización familiar | que la persona tiene permiso familiar para inscribirse | datos de prueba: una persona con autorización; otra no |
| Validación de datos no válidos | que la edad sea un numero positivo, y que no supere los 120 | -5; 0; 121; 145 |
| Resultado final de inscripción | una vez introducidos los datos, que se permita al usuario inscribirse | se debe hacer una prueba de caja negra completa |
### Casos de prueba iniciales
   ID,Funcionalidad,Datos de entrada,Resultado esperado
CP-001,Validación de edad mínima,11,“El usuario tiene que ser mayor de 12 años”
CP-002,Validación de edad mínima,12,“Edad válida”
CP-003,Validación de edad mínima,15,“Edad válida”
CP-004,Validación de edad máxima,19,“El usuario no puede ser mayor de 18 años”
CP-005,Comprobación de autorización familiar,Usuario sin autorización,“El usuario necesita una autorizción familiar”
CP-006,Comprobación de autorización familiar,Usuario con autorizacion,“Autorización válida”
### Respuestas razonadas
  • ¿Por qué no conviene probar únicamente edades claramente válidas, como 15 o 16  años?

Porque no forza el programa a enfrentar situaciones atípicas que en la vida real pasan mucho.

• ¿Qué valores límite aparecen en este programa?

18; 12; 120 por ejemplo serían valores límite


• ¿Por qué es importante probar tanto personas con autorización como sin autorización?

Para asegurarnos de que se ha implementado la validación de tener o no autorizacion


• ¿Qué datos no válidos habría que tener en cuenta?

Edades invalidas, usuarios no autorizados

• ¿Qué ventaja tiene planificar estas pruebas antes de ejecutar el programa?

Ahora ya se saben los puntos de inflexión de programa; están localizadas sus debilidades que se probarán repetidas veces a lo largo de su desarrollo


