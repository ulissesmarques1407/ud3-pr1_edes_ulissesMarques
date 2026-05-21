# Bloque 1 - Introducción a las pruebas
## Tarea 1: primera reflexión sobre pruebas
         Situación
Dato de entrada
Resultado que debería obtenerse
Pedido inferior a 50 € de cliente normal
35€
40€
Pedido exactamente de 50 € de cliente normal
50€
50€
Pedido superior a 50 € de cliente normal
51€
51€
Pedido inferior a 50 € de cliente premium
40€
36€
Pedido con importe negativo
-1
InputMismatchException


### Respuestas razonadas
          Después de la tabla, responde de forma razonada:
 • ¿Sería suficiente probar solo con un pedido de 100 €?
Por supuesto que no; realisticamente no cubre todas las facetas del código y posibles defectos  errores
 • ¿Por qué es importante probar el caso de exactamente 50 €?
Por si hay un algún fallo en el parámetro específico de que puede ser mayor o igual  a 50€
 • ¿Qué diferencia hay entre probar un dato válido y un dato no válido?
Vemos como se comporta o programa en ambas situaciones
 • ¿Qué podría ocurrir si el programa no controla importes negativos?
Directamente nos saltaría un error de ejecución; se interrope el programa, una excepción
 • ¿Por qué comprobar que un programa “parece funcionar” no es suficiente?
Porque “funcionar” es una palabra muy ampla: pocos programas realmente funcionan; es necesario testar exhaustivamente en cuanto a todo que uno no se espera que pueda pasar.
