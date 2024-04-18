#tutorial introductorio a python
##variables parte2;  funciones para las variables, formateo y concatenación
###introducción
¡bueno, bueno! trás 30 años de tardanza, regreso con un nuevo aporte a este tutorial.

para empezar, quiero pedir una disculpa, y agradeceros a los que de vez en cuando revivíais esto, el interés se agradece mucho.

también quiero decir que estoy siguiendo la encuesta, y el 79% fue esto, así que nada, pongámonos a explicarlo. espero que en poco tiempo (menos de los  meses que tardé en escribir esto) llegue el capítulo 3
sin nada más que añadir para esto, sean vienvenidos y demos comienzo

###funciones para las variables.

para empezar, una función es un pedazo de código que te permite realizar una acción tantas veces como quieras en cualquier lado del código. aplicado a un juego, digamos que tienes la función para saltar, la cual la puedes usar cada vez que tu personage deba saltar. sin o, tendrías que escribir el código del salto cada vez que lo requieras, cosa la cual sería engorrosa.

esto se explicará de una mejor manera en la parte referida a las funciones, que será aproximadamente según mis cálculos el capítulo 4 o 5.

bién, entendido por encima que son las funciones, ahora hablemos de las funciones para las variables. tenemos varias, entre ellas las siguientes, que serán las que aprenderemos.

- len()
  - te da el  tamaño de la variable; útil sobre todo por ejemplo para evaluar si una variable tiene más de un número. o menos de el, como por ejemplo para las contraseñas.
- format()
  - ayuda a insertar una variable u otro contenido dinámico en la variable o función (por ejemplo, print). lo veremos a fondo en formateo y concatenación.

ahora, veamos un ejemplo de cada una de ellas.

- para len:

```python```

variable="hola, esta es una variable de prueba."
print("el tamaño de la variable es:")
print(len(variable))

el output que recivimos es algo como

>>el tamaño de la variable es:
>>37

esta función lo que hace es ver el número de bits guardados en la variable, lo que para nosotros se traduce en caracteres. por lo tanto, aquí tenemos 37 caracteres, con todo y espacios, comas y puntos. es importante que entendamos eso para saver usarla al momento de introducir límites para un campo de texto, para un cuadro de contraseñas etc.
- para format:

esto lo veremos más a fondo en concatenación (el siguiente apartado) pero en síntesis, no deja de ser una forma de concatenar. lo que vimos antes metiendo una función dentro de un print, también aplica para concatenar o poner variables. python tiene varios métodos de concatenarlas, pero los más usados y los mejores (almenos a mi parecer) son las formated strings y la función.format, que son las que veremos en este tutorial.

la función.format, de la que hablaré en concatenación, se ve tal que así.

variable="vamos a formatear una variable"

print("la variable dice lo siguiente: {}.".format(variable))

el output recivido debe ser similar al siguiente:

>>la variable dice lo siguiente: vamos a formatear una variable.

como pueden ver, aquí en el texto de salida, tenemos el texto de la variable. esto sirve por ejemplo para hacer el código mas pequeño, cuando hay que imprimir mas datos. visualmente también cambia un poco la cosa, aunque de esto no hablaré tanto por desconocimiento tanto como por que el rumbo de este tutorial no va hacia ahí. de todas formas, si interesa mucho el tema de los cambios visuales entre prints, y concatenación con .format o con formated string, lo investigaré y os contaré.

###concatenación de variables y formateo

para concatenar variables, hay varias formas. para una sola variable o algo sencillo, existe el método mas simple de todos, y que en cierta medida es similar a la forma de hacerlo en otros lenguages:

variable="vamos a formatear una  variable"

print("la variable dice: ", variable)

el output que deberías recivir es:

>>la variable dice: vamos a imprimir una variable


pero esto, pese a ser funcional, no lo veo como la mejor opción si necesitamos meter varios datos. lo es, claro, si el lenguage no te ofrece otra medida, pero teniendo las formated strings es una tontería usarlo de esta manera.

**¿que son las formated strings?**

las formated strings, se parecen al.format que ya conocemos. la diferencia en este caso es que no necesitas poner todas las variables en la función, si no en el pedazo del código que les pertenecen. es decir. la función punto format sirve, pero imaginad que teneis que hacer un output que contenga muchos datos de muchas variables, tal como un print para listar las versiones de windows, los módulos necesarios que cambien, u otro tipo de cosas en una de las aplicaciones. format  serviría si, pero tendrías que poner todas las variables en la función, lo cual puede resultar engorroso y vastante extraño para una persona que lea nuestro código y no sepa nada.

para eso existen las formated strings. estas se declaran poniendo una "f" antes de abrir las comillas, y tras ello, cualquier variable que quieras poner solo debes ponerla entre las llaves.
veamos un ejemplo.


variable="esto es una variable concatenada por formated strings."


print(f"hola. en este ejemplo, vemos una variable concatenada por formated string. la variable dice: {variable}. ¡saludos!")

el output que optenemos es:

>>hola. en este ejemplo, vemos una variable concatenada por formated string. la variable dice: esto es una variable concatenada por formated strings.. ¡saludos!


esto en algunas ocasiones incluso sirve  para meter código dentro de las llaves, de tal manera que tengamos menos líneas de código nosotros en nuestro programa, pero esto lo veremos en tutoriales más avanzados. no por nada, simplemente es que yo tampoco se como funciona esa parte en espefícicco

#conclusión

Como podemos ver, python es un lenguage hermoso, y me alegra que os guste esta iniciatiba. escribo esta conclusión para pedir unas sinceras disculpas por mi tardanza, intentaré que no vuelva a pasar, de verdad.

les deseo  suerte.  un saludo, y observarán que esta vez no hay ejerficios de práctica. esto es devido a que el ejerficio simplemente consta de lo siguiente:

- crea un programa simple en python, con lo ya aprendido hasta ahora. utiliza inputs, variables, y prints. pero a la ora de concatenar información, usa todos los métodos mostrados en este tutorial.

¡chao!