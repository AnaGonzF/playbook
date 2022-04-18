# Weekly Mission 1

Esta primera semana vimos muchos ejemplos sobre JS, sobre todo para poder entender la lógica del mismo, además de meternos también a Node.

Aquí dejo mi ruta de aprendizaje. :)

## Primeros pasos

Para comenzar, me vi algunos tutoriales sobre el control de versiones, Git, ya que al tener Windows no podía realizar esto desde la consola, además de que no conocía cómo funcionaba Git. Entonces comencé a ver de qué trataba, así también podía resolver las dudas de mi workbook.

Aquí el link de los videos que utilicé para poder familiarizarme y entender mejor Git:

[¡Aprende Git ahora!](https://www.youtube.com/watch?v=VdGzPZ31ts8)

[Consola Linux en Windows 10](https://www.youtube.com/watch?v=J9LPuCgDAVk)

[Installing and customizing The Fish Shell]()

Y para complementar el tema de JS, vi el siguiente video:

[Curso JavaScript para principiantes](https://www.youtube.com/watch?v=RqQ1d1qEWlE)

En la primera parte y como una prueba para ver si realmente estaba instalado Node, realicé un archivo JS y lo corrí en la consola para verificar que todo estuviera en orden.

[Este fue el archivo para probar](https://github.com/AnaGonzF/playbook/blob/main/weekly_mission_1/hello.js)

Aquí el resultado en consola:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/hello_js.png">

## Ejemplos

Aquí comenzamos con los ejemplos realizados para familiarizarme y entender JS.

### Example 1: Objetos de JS

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_1)

Aquí el resultado del ejemplo 1 en consola:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/example_1%20main_js.png">

En este ejemplo se observa más que nada qué es un objeto, para qué sirve, como se crea, sus propiedades, cómo se le declaran variables y el uso de return para exponerlas.

### Example 2: Exportando funciones entre scripts con CommonJS

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_2)

Aquí el resultado del ejemplo 2 en consola:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/example_2%20main_js.png">

En este ejemplo es sobre todo para exportar.

En el archivo *logger.js* se guardó una función de mensaje como info y otra como verbose, para que en el archivo *main.js* se requiera el *logger.js*, se coloca la función *require*, se colocan las funciones del archivo *logger.js* para llamarlas y añadiendo el mensaje escrito que queremos que se lea. 

Esto nos ayuda con la modulación.

### Example 3: Diferentes formas de exportar funciones

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_3)

Aquí imagen de cómo se ve en consola el ejemplo 3:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/example_3%20main_js.png">

En este ejemplo se usaron dos archivos logger, *logger_1**.js* y *logger_2.js*, y un solo *main.js*.

En los archivos *logger_1.js* y *logger_2.js* se observa nuevamente cómo se declara una función para llamarla en otro script junto con el mensaje que queramos, en esta ocasión dividimos las funciones *info* y *verbose*, para seguir viendo que podemos modularizar. 

Y por último (cómo en los anteriores ejercicios), pero no menos importante, usamos *main.js* para llamar las funciones y asignarles el mensaje.

### Example 4: Clases y objetos

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_4)

Ejemplo 4 en consola:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/example_4%20main_js.png">

En este ejemplo usamos los archivos *logger.js* y *main.js*.

En *logger.js* se usó una clase llamada Logger, esta clase contiene una variable *constructor* y una *this*, esta última nos ayuda para referenciar el valor del contexto local de la clave.

Después se vuelven a usar las funciones info y verbose, como método, dentro de la clase aún y finaliza con la ecportación.

En el archivo *main.js*, llamando a la clase con require. Después se crea un objeto para llamar al constructor de la clase y se le agrega el mensaje. Así mismo se crea otro objeto con un mensaje vebose.

### Example 5: Clases y objetos

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_5)

Ejemplo 5 en consola:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/example_5%20main_js.png">

En este ejemplo tenemos los archivos *logger.js* y *main.js*.

Nuevamente se usa una clase para poder tener dentro dos objetos: *constructor* y *log*, con sus respectivos valores y métodos, para finalmente instanciarlos y mandarlos a *export*.

### Example 6: Modificación de clases

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_6)

Aquí la ejecución del ejemplo 6 en consola:

<img width="1247" alt="image" src="https://raw.githubusercontent.com/AnaGonzF/playbook/main/weekly_mission_1/Resources/example_6%20main_js.png">

En este ejemplo tenemos los archivos *logger.js*, *patcher.js* y *main.js*.

Para este ejemplo se usa nuevamente una clase en el archivo de logger que contiene dos objetos, su instancia y la exportación.

En el archivo patcher.js se le agrega una función al objeto instanciado de la clase Logger en el archivo logger.js.

Para finalizar, se llama al módulo que modifica la función (*patcher.js*) y luego al módulo que tiene el objeto a modificar (*logger.js*).

### Example 7: EcmaScript Modules ESM

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_7)

Aquí el ejemplo 7 en consola:

<img width="1247" alt="image" src="https://github.com/AnaGonzF/playbook/blob/main/weekly_mission_1/Resources/example_7%20mains_js.png?raw=tru">

En este ejercicio tenemos los archivos *package.json*, *logger.js*, *main_module.js*, *main_2.js* y *main.js*.

Aquí observamos que se tiene un paquete *json* que contiene información sobre "*esm-sytanx*".

El módulo logger.js se comporta como si guera un objeto que tiene todo lo definido. Exporta función, constante, un objeto y una clase, todo con información sobre "*esm-sytanx*".

La función de *main_module.js* es importar el modulo.

Y en los archivos *main.js* y *main_2.js* se importa *logger.js* para así ver la info con ayuda de *console.log()*.

### Example 8: EcmaScript Export Default

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_8)

Ejemplo 8 en la consola:

<img width="1247" alt="image" src="https://github.com/AnaGonzF/playbook/blob/main/weekly_mission_1/Resources/example_8%20main_js.png?raw=true">

En este ejemplo usamos los módulos *package.json*, *logger.js*, *main_2.js* y *main.js*.

Nuevamente se usa el paquete de *package.json* con el mismo contenido.

En logger.js se exporta e importa la clase logger. Y finalmente en main.js y ,ain_2.js se observan con sus respetivos mensajes.

## Ejercicios

### Example 9: Ejercicio

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_9)

***Cooming soon in next updates...***


Example 10: Ejercicio

[Example in GitHub](https://github.com/AnaGonzF/playbook/tree/main/weekly_mission_1/example_10)

***Cooming soon in next updates...***



## Uso de Git

Aquí un ejemplo de cómo he hecho uso de git en mi playbook.

<img width="1247" alt="image" src="https://github.com/AnaGonzF/playbook/blob/main/weekly_mission_1/Resources/Ejemplo%20de%20mi%20uso%20de%20git%20.png?raw=true">
