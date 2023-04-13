## ¿Que són las memory leaks?

Las "memory leaks" o fugas de memoria son un problema común en muchos programas, incluyendo videojuegos. Ocurren cuando un programa no libera correctamente la memoria que ha asignado durante su ejecución, lo que puede llevar a que el programa consuma cada vez más memoria a medida que se ejecuta, hasta que finalmente se agota toda la memoria disponible en el sistema y el programa se bloquea o se cierra.

En los videojuegos, las memory leaks pueden ser especialmente problemáticas, ya que los juegos a menudo requieren grandes cantidades de memoria para funcionar correctamente. Si un juego tiene una fuga de memoria, puede llevar a que se reduzca el rendimiento, a problemas de estabilidad o incluso a que el juego se cierre inesperadamente.

Para prevenir las memory leaks en los videojuegos y otros programas, los desarrolladores deben asegurarse de liberar correctamente la memoria que asignan durante la ejecución del programa, lo que implica identificar y corregir cualquier problema de gestión de memoria que pueda estar presente.

## ¿Que producen las memory leaks?

Las "memory leaks" o fugas de memoria en los videojuegos pueden producir una serie de problemas, algunos de los cuales incluyen:

- Reducción del rendimiento: A medida que el programa consume más y más memoria, puede volverse más lento y menos sensible, lo que puede llevar a una disminución en la tasa de fotogramas, lo que se traduce en una experiencia de juego menos fluida.

- Problemas de estabilidad: Si un programa consume demasiada memoria, puede agotar los recursos del sistema y causar que el programa se bloquee o se cierre inesperadamente.

- Errores y comportamiento inesperado: Las memory leaks pueden causar comportamientos inesperados en los videojuegos, como errores gráficos o problemas de colisión.

- Problemas de guardado: Si el juego no puede liberar correctamente la memoria asignada, puede haber problemas al guardar el progreso del jugador, lo que puede llevar a la pérdida de datos.

- Dificultades para depurar: Si hay una fuga de memoria en el juego, puede ser difícil de detectar y corregir, especialmente si ocurre de manera intermitente o en circunstancias específicas.

Por lo tanto, es importante para los desarrolladores de videojuegos asegurarse de evitar las memory leaks en sus juegos, para garantizar una experiencia de juego estable y fluida para los usuarios.

## Cómo detectarlas y solucionarlas

Hay varias formas de detectar las "memory leaks" o fugas de memoria en los videojuegos y otros programas. Algunas de las técnicas más comunes incluyen:

- Pruebas de estrés: Las pruebas de estrés pueden ayudar a detectar las memory leaks en los videojuegos. Los desarrolladores pueden ejecutar el juego durante un período prolongado de tiempo y observar el consumo de memoria del sistema para detectar cualquier aumento significativo en el uso de memoria.

- Perfilado de memoria: Las herramientas de perfilado de memoria permiten a los desarrolladores ver cómo se está utilizando la memoria en el juego. Esto puede ayudar a identificar cualquier área problemática que pueda estar causando una fuga de memoria.

- Herramientas de análisis de memoria: Utilizar herramientas de análisis de memoria: Las herramientas de análisis de memoria, como Valgrind, pueden ayudar a detectar las "memory leaks" en el código del programa. Estas herramientas pueden señalar las partes del código que no están liberando correctamente la memoria y ayudar a los desarrolladores a corregir el problema.

- Pruebas manuales: Los desarrolladores también pueden realizar pruebas manuales en el juego para detectar cualquier problema de memoria. Esto puede incluir la realización de pruebas específicas en áreas del juego que tienden a consumir mucha memoria.

- Liberar la memoria correctamente: Es importante asegurarse de que la memoria se libera correctamente en el código del programa. Los desarrolladores pueden utilizar las funciones de liberación de memoria adecuadas, como "free" en C y C++, para liberar la memoria asignada.

Es importante tener en cuenta que la detección de "memory leaks" puede ser un proceso complejo y que la identificación de un problema de fuga de memoria no siempre es sencillo. Por lo tanto, es fundamental realizar pruebas rigurosas y utilizar herramientas adecuadas para identificar y corregir cualquier problema de fuga de memoria antes de que afecte al rendimiento del juego.

## Softwares de detección de Memory leaks

Existen diversas herramientas de perfilado de memoria que se pueden utilizar para analizar el comportamiento del uso de memoria en programas y videojuegos. Algunas de las herramientas de perfilado de memoria más populares son:

- Valgrind: Es una herramienta de análisis de memoria que puede detectar y reportar problemas como "memory leaks", uso no inicializado de la memoria, errores en el acceso a la memoria, entre otros.

- Visual Studio Memory Profiler: Es una herramienta de perfilado de memoria para aplicaciones de Windows que se integra en el entorno de desarrollo de Microsoft Visual Studio. Proporciona información detallada sobre el uso de memoria y puede ayudar a identificar problemas de "memory leaks".

- JetBrains dotMemory: Es una herramienta de perfilado de memoria para .NET que proporciona información sobre el uso de memoria de una aplicación. Puede identificar objetos que no se están liberando adecuadamente y proporcionar información detallada sobre su uso.

- Intel VTune Amplifier: Es una herramienta de análisis de rendimiento que también incluye una funcionalidad de perfilado de memoria. Proporciona información detallada sobre el uso de memoria y puede ayudar a identificar problemas de "memory leaks" y otros problemas de rendimiento.

Estas son solo algunas de las herramientas de perfilado de memoria disponibles en el mercado. Los desarrolladores pueden elegir la herramienta que mejor se adapte a sus necesidades y que les ayude a detectar y solucionar problemas de "memory leaks" y otros problemas de rendimiento en sus programas y videojuegos.

A continuación, os explicaré cómo utilizar Valgrind para detectar y solucionar "memory leaks" en tu código:

1. Instala Valgrind: Para utilizar Valgrind, primero debes instalarlo en tu sistema. Puedes hacerlo a través del gestor de paquetes de tu sistema operativo o descargándolo directamente desde la página web de Valgrind.

2. Compila el código con las opciones de depuración: Para poder utilizar Valgrind, necesitas compilar el código del programa con las opciones de depuración habilitadas. Esto permite que Valgrind tenga acceso a información adicional sobre el uso de memoria en el programa.

3. Ejecuta Valgrind: Una vez que el programa está compilado con las opciones de depuración habilitadas, puedes ejecutar Valgrind en el código utilizando el comando "valgrind" seguido del nombre del programa y cualquier argumento que necesite el programa. Por ejemplo:

4. Analiza el reporte de Valgrind: Después de que Valgrind haya ejecutado el programa, producirá un informe detallado que mostrará cualquier problema de "memory leaks" que haya detectado. Deberás analizar cuidadosamente el informe para identificar los problemas y solucionarlos.

5. Corrige los problemas de "memory leaks": Una vez que hayas identificado los problemas de "memory leaks" en el informe de Valgrind, debes corregirlos en el código del programa. Puede implicar modificar la forma en que se asigna o libera memoria en el programa.

6. Vuelve a ejecutar Valgrind: Después de realizar las correcciones, vuelve a compilar el programa con las opciones de depuración habilitadas y ejecuta nuevamente Valgrind para asegurarte de que los problemas de "memory leaks" hayan sido solucionados.

## Implementación en proyecto

En nuestro proyecto utilizaremos técnicas manuales y si nos vemos con la carga de que hay cosas con las que no podemos lidiar, utilizaremos el Software de Valgrand. 

Actualmente no hemos utilizado el software, pero después de haber hecho el estudio de su respectivo uso, y cómo aplicarlo a nuestro proyecto, nos veremos obligados en diversas situaciones a utilizarlo.

Explicación de su uso en diversos ámbitos en la presentación.

## Debate (Manual o Software?)

Ahora mismo entraremos en un debate entre sí es mejor recorrerlo todo a ojo o no.

Sinceramente, depende. Sí son errores de lógica muy básicos, se pueden hacer a ojo, al igual que liberar la memoria. Pero yo desde mi punto de vista y lo que haremos en nuestro proyecto es utilizar los dos métodos, tanto las técnicas de detección manual como los software

