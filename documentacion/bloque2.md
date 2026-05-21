# Bloque 2 - Tipos de pruebas
## Tarea 2: clasificación de tipos de pruebas
   
| Caso | Tipo de prueba principal | Justificación |
| --- | --- | --- |
| Ejecutar un programa de venta de entradas e introducir una entrada de 12 € para comprobar que calcula correctamente el precio final. | prueba caja negra | se prueba el programa desde la perspectiva "de fuera"; de usuario |
| Comprobar que un programa de cálculo de becas devuelve “concedida” cuando la renta está por debajo del límite establecido. | prueba caja negra | se enfoca en verificar el comportamiento del programa según las especificaciones |
| Revisar el código de un método y diseñar pruebas para que se ejecute tanto el if como el else. | caja blanca | sólo se centra en un aspecto interno del programa y lo prueba separadamente del resto |
| Volver a ejecutar todas las pruebas después de corregir un error en el cálculo de una calificación. | regresión | posteriormente a algún cambio se prueba todo el programa por si hay algún conflicto |
| Comprobar directamente un método llamado calcularMedia usando varios valores de entrada, sin ejecutar todo el programa completo. | unitaria | sólo se centra en un método del programa |
| Introducir una edad negativa para comprobar si el programa la rechaza. | validación de datos | manualmente se introducen todo tipo de datos buscando anomalías en el programa |
| Ejecutar manualmente un programa desde la consola e ir anotando los resultados obtenidos. | caja negra, manual | se testea el programa manualmente, desde la perspectiva del usuario |
| Ejecutar una batería de pruebas ya preparada sin introducir los datos manualmente. | prueba automática | diseñada para ahorrar tiempo y hacer pruebas específicas |
### Primeros datos de prueba

| Dato de prueba | Tipo de caso | Resultado esperado |
| --- | --- | --- |
| 4.5 | Caso válido inferior al límite | no apto |
| 5 | Caso justo en el límite | apto |
| 9 | Caso válido superior al límite | apto |
| -1 | Caso no válido por debajo del rango | dato no válido |
| 14 | Caso no válido por encima del rango | dato no válido |
### Respuestas razonadas
  • ¿Qué diferencia hay entre una prueba funcional o de caja negra y una prueba estructural o de caja blanca?

La perspectiva: la de caja negra mira al programa desde fuera desde la perspectiva del usuario; la de caja blanca es interna, estructural

 • ¿Por qué las pruebas de regresión son importantes cuando se modifica el código?

Porque es muy típico que alguna actualización en el código, sobretodo si fruto de trabajo ajeno, se choque con el código escrito previamente.

 • ¿Qué ventaja tiene una prueba automática frente a una prueba manual?

La prueba automática se puede calibrar para un objetivo en concreto y ejerce su función de forma rápida y dinámica; se ahorra tiempo,  es reciclable, y tiene mayor escalabilidad

 • ¿Por qué una prueba unitaria puede ayudar a localizar mejor un error?

Porque aisla elementos específicos del código; es excelente para localizar errores en estructuras relativamente complejas

 • ¿Por qué no debemos probar solo datos válidos?

Porque realisticamente el programa estará completamente expuesto a todo tipo de dato absurdo: tiene que estar preparado!


