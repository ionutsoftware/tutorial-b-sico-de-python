# Tutorial Introductorio a Python
## Capítulo Dos: Las Variables - ¿Qué son? ¿Cómo les añado información? ¿Puedo cargar información por teclado con variables?

¡Hola gente, y bienvenidos seáis una vez más a un nuevo capítulo de este tutorial! Hoy es viernes, y una semanita más tarde volvemos con el tutorial, además de con este capítulo que en especial es sencillo, pero al mismo tiempo difícil. Las variables en Python (y en cualquier lenguaje), pero especialmente en Python, son extremadamente sencillas. Sin embargo, la gente no suele comprender al principio lo que son, así que en este capítulo también tendremos ejercicios a completar en vuestra casa. ¡Sí, tendremos deberes! ¿Pensábais libraros? ¡Pues no!

Dicho esto, vayamos a empezar con el capítulo.

### Las Variables - ¿Qué son?



En síntesis, una variable es un contenedor de carga en un gran barco. Estos contenedores sirven para poder cargar información y poder acceder a ella o incluso cambiarla de posición o cantidad.
Un ejemplo muy claro de una variable es, tomando como ejemplo un juego, la sed, el cansancio o la energía (que no se note que hago referencia a STW, por favor).
Estas tres son variables, las cuales cambian. ¿Imaginas tener que cambiar manualmente para cada usuario su sed, su hambre, su sueño? Sería una total pesadilla, y por supuesto, subirían tan lentamente o bajarían tan lentamente que tendríamos una lista de espera.
Entonces, las variables sirven para almacenar la información y cambian según sea el caso. Pero, ¿cómo es una variable?
Pues, vayamos a ver un ejemplo:
`python`

nombre = "juan"

edad = 35

peso = 60,5


print("nombre:")

print(nombre)

print("edad:")

print(edad)

print("peso")

print(peso)


como podeis ver, aquí vemos líneas de código. vallamos a aclarar unos cuantos términos antes de ver lo que hacen estas líneas:

###tipos de variables:

en el código anterior, podemos ver diferentes tipos de variables. unas que tienen comillas, otras que no... ¿porqué? pues, por que en si, son tipos de variables diferentes.

en cualquier lenguage, para poder tener un código organizado, un mejor control hacerca de los datos y algunas cosas complicadas que veremos probablemente al final de este curso, cuando lla sepamos todo lo necesario para trabajar con datos, se utilizan diferentes tipos de variables. haver, hay vastantes, pero al final, vamos a citar a las más importantes que serán las únicas que se utilizarán en realidad.

en python, no hace falta mencionar el tipo de variable que usarás. a diferencia de otros lenguages, python detecta automáticamente las variables que son por su contenido y te permite no tener que indicarlas, lo cual es en cierto modo un veneficio, por que te simplifica el código, pero es difícil para la gente que comienza porque no ves que variable es, y quizá (dependiendo de la persona) cueste un poco más distinguirla.

entre las variables podemos encontrar:

- string:

las variables de tipo "string" son variables que contienen texto. "string" en inglés significa cadena, y lo que estas variables procesan es una cadena de caracteres, tales como un texto, una palabra, una letra o una sílaba.

un ejemplo de variable de tipo string podría ser, viendo nuestro código anterior:

nombre = "pedro"

analizemos la línea:

- nombre: aquí nombramos la variable, en este caso el nombre es "nombre" para saver que esta variable almacena un nombre. se recomienda poner nombres completos a las variables, para poder saver tras mucho tiempo de no trabajar en su código que hacía esa variable concreta.


- =: "el símbolo "="(igual) se utiliza para que nuestro intérprete sepa que a continuación vamos a asignarle un valor a la variable, es decir. digamos que en nuestro contenedor, el igual sería la tapa. por arriba tiene el nombre, y por debajo el contenido.

- "nombre": contenido de las variables. en este caso, esta es una variable de tipo string, la cual contiene una cadena de caracteres. siempre que pongamos texto en un código, ya sea por un mensage en la pantalla, por un contenido de una variable, etc, se pone entre  "(comillas) esto sirve para que nuestro intérprete sepa que lo que  viene a continuación es texto. si no, lo trataría como código y optendríamos un error como:



```python

print(hola)

>>>Traceback (most recent call last):
  File "<console>", line 1, in <module>
NameError: name 'hola' is not defined

si hacemos eso, lo que pasará es que nuestro intérprete  entenderá que "hola" es un argumento de una función, o una variable. si ponemos algo sin las comillas en una cadena, se entenderá que es otra cadena (string) o un argumento de una función.


- int:

int(por su nombre completo en inglés, integer) son variables que solo aceptan números, enteros. su nombre en español se traduciría literalmente como entero, y por lo tanto, solo acepta números enteros, tales como "1, 2, 3, 222".

analizemos un int de nuestro código:

```python


edad = 35


analizemos:

- edad:  al igual que en la variable anterior, añadimos un nombre a la variable.

: = lo mismo que en el anterior, le indicamos al código que de aquí en adelante viene el contenido del contenedor.

- 35: indicamos el número de años que tiene, es decir, el contenido de la variable que es un número. como podemos observar, esta variable no necesita comillas. si pones  comillas en una variable de tipo int, lo  único que pasará es que la tomará como string, y que si intentas hacer operaciones matemáticas con ella (ahora os enseñaré también a usar python de calculadora) dará un error como este.

n1= "20"

n2 = "30"

res=n1-n2


Traceback (most recent call last):
  File "<console>", line 1, in <module>
TypeError: unsupported operand type(s) for -: 'str' and 'str'

básicamente nos dice que no se puede operar con ellos, que no puedes operar con un -(menos) dos operadores de tipo string (str)



vien, dicho esto, vallamos al siguiente tipo de variable:

- variables de tipo float (flotantes):


imagina  que necesitas establecer el peso de un jugador, o de una persona. el peso nunca es  entero, o casi nunca. pocas veces tenemos 50 kilogramos enteros, o 200 gramos de carne, o lo que querais decir. en su lugar podemos tener 50,3 kilogramos, 200,1 gramos de carne... y una variable entera no podría  soportar eso. tampoco nos toparemos con equivocarnos de variable en python, pero podemos provocar a drede la comfusión para ver el error. python tiene una función que nos comvierte todo a entero, o a flotante (eso es otra función) así que hagamos la prueba.

variable=int(90,3)


Traceback (most recent call last):
  File "<console>", line 1, in <module>
TypeError: int() can't convert non-string with explicit base

daría un error. pero i si vemos una float normal?


peso = 90,3

la variable no devería devolver ningún problema. es así como python reconoce el tipo de variables, y nos haría técnicamente imposible equivocarnos, amenos que forcemos la comversión.


finalmente, tras establecer las variables, podemos imprimirlas usando print. para ello, utilizamos print, y como argumento (entre los paréntesis) le ponemos los nombres de las variables sin comillas. de ponerlo con comillas, lo único que obtendríamos sería el nombre impreso en pantalla.


###carga de datos por teclado en python

como se habrán dado cuenta, muchas veces no solo tendremos variables que se rellenen automáticamente, también necesitamos datos de un usuario, como (volviendo a nuestro juego) el nombre de usuario, la cantidad de items que quiere comprar de la tienda, y un largo etcétera.

para ello tenemos nuestra función del motor python para pedir datos por teclado a nuestro usuario, y luego convertirlos en lo que queramos, o imprimirlos o... simplemente usarlos.

esta función es input

la función se vería así:

```python

var=input(text)

ahora, expliquemos este código que no tiene lógica.

primeramente, declaramos una variable. ¿porqué? pues, si vas a pedirle datos al usuario, necesitas un lugar donde guardarlos, ¿no? si no esos datos no servirán de nada, y tu esfuerzo por adquirirlos se perderían pues el input sería un solitario pedazito de código. una variable (nuestro contenedor) se encargará de que tal desgracia no suceda, y guardará nuestra información. tenemos un solo tipo de input, y un montón de tipos de datos que se pueden introducir, pero como podemos asegurarnos y rectificar en cada caso lo veremos en el próximo capítulo.

luego, declaramos el input. input, traducido a nuestro idioma (el español) significaría entrada. y es precisamente lo que hace. nos permite entrar datos por teclado.


un input real se vería como:

```python```

text=input("introduce un texto aquí")

print(text)

como puedes ver si ejecutas ese código, te pedirá un texto. tras dar enter, este se imprimirá en pantalla.

primero declaramos el input:

text=input("introduce un texto")

aquí declaramos una variable para que contenga el texto, y en el input tenemos un solo argumento, el cual es lo que le pedimos al usuario. también podríamos poner una variable por input, pero perdería la gracia a menos que necesitemos meter datos cambiantes, cosa que veremos cuando lleguemos al formateo de la variable.

print(text)

declaramos la ya conocida función print, y le pasamos por parámetro nuestra variable.

bueno, hasta aquí el tutorial de hoy. lamento la tardanza, pero he estado muy ocupado estas semanas con la escuela.

se que no está tan completo como desearan, pero tengo que entregar un capítulo, y prometo que el siguiente incluirá mas datos.


##ejerficios.

¡hey! ¿a donde vas?

todabía no hemos terminado. se que pensaste que te irías sin deberes, pero como profesor duro que soy no lo puedo permitir. a continuación viene una lista de ejerficios que quiero que hagais y lo pegueis en este hilo, para que os pueda corregir si stán mal, o felicitar si están bien:

- ejerficio 1: crea un programa con 3 variables:
  - nombre
  - edad
  - peso
  luego, imprímelas.


- crea un programa donde solicites lo siguiente:
  - nombre
  - edad
  - peso
  - y finalmente, algo que la persona uqiera decir.
  imprime todo.

- siéntete libre de hacer libre tu imaginación. crea programas fuera de los ejerficios que yo te di, y ejercita tu mente en python. si hay algo que quieras compartir, ¡estaremos encantados de verlo!