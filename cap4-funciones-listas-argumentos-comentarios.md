#tutorial introductorio a python
##capítulo4; un vistazo a los comentarios, a las funciones y a los argumentos

###introducción:
¡buenas a todos, todas y todes!
han pasado 2 mesecitos, y viendo que alguien (pocos pero alguien) me pidió que continuase con esto pues continuaré.
¿que veremos hoy?

¡perfecta pregunta!

hoy veremos lo más esperado (almenos por mi) de todo el tutorial, por que así se simplificará el entendimiento de todo lo que veremos a futuro. la mayoría de módulos tienen funciones, y en muchísimas ocasiones necesitarás usar listas. diccionarios también, pero esos van para el capítulo que viene, osea probablemente en junio o algo así.

haver, en realidad en los módulos llamas a objetos de una clase, pero en síntesis son funciones también, solo que se mencionan de diferente forma en un código.
pero pasemos ya al curso, por que si no puedo pasarme 3 siglos y medio hablando en la introducción.

####funciones

empezemos por lo primero, y lo más sonado devido a que hablamos de ello casi desde el principio de este tutorial.


las funciones.
como ya expliqué en inumerables ocasiones, las funciones son pedacitos de código que sirven para ser repetidos de forma sencilla en mas lugares del código, o para ordenarlo.

no es lo mismo escribir todo tu código como hicimos hasta ahora, en un solo documento, y de forma desorganizada o sin ningún tipo de estructura ha hacerlo con funciones. veamos un ejemplo relativamente sencillo.

no es lo mismo hacer lo siguiente:
```python

nombre-archivo=""
contenido-archivo=""
with open(nombre-archivo", "w") as archivo:
    archivo.write(contenido-archivo)

a esto:
```python

def crear_archivo(nombre-archivo, contenido-archivo):
    with open(nombre-archivo, "w") as archivo:
        archivo.write(contenido-archivo)

como podemos ver, mientras que en la primera especificamos 2 variables en el código (no las inicialicé por que solo era un ejemplo, pero podrías poner nombre y contenido entre las comillas y funcionaría igual), en la segunda hice una función. el resultado es el mismo, creamos un archivo. (hablaremos de with open, de las palabras as, or, y demáses en otro capítulo) pero por ahora centrémonos en esto.
la diferencia entre la primera y la segunda es que mientras que para realizar la creación de un archivo en la primera situación, cada vez que desearía crear un archivo debería escribir todas las líneas de código, haciendo un código estorboso y largo, en la segunda, simplemente debería hacer:

```python

crear_archivo("nombre.txt", "escribiendo")

y podría reusar esta línea para crear todo tipo de archivos. en un juego, podría ser útil para crear archivos en la carpeta, para crear el archivo.ini... aunque no solo se pueden hacer este tipo de cosas con las funciones. puedes hacer de todo. desde hacer que tu personage salte en un juego, hasta hacer una función como speak para hacer que nvda hable usando un módulo como cytolk o pyxtts3 o el accesible_output (pero los pythondevs me matan si lo pongo de ejemplo, por que "está descontinuado y obsoleto")
de la importación de módulos hablaremos en el capítulo 6, antes tengo que daros las condicionales

bueno, la cosa es que una función sirve para hacer todo tipo de cosas.

tenemos varios tipos de funciones, aunque en general, se dividen en 2:

- funciones con argumentos.
- funciones sin argumentos.

#####funciones con argumentos

una función con argumentos puede ser perfectamente la del ejemplo anterior. en si, los argumentos de la función se usan cuando sirven para crear algo en base a una entrada del usuario, o cuando son dinámicas, es decir, no siempre sirven para lo mismo. una función estática, siempre hará lo mismo. por ejemplo, tomando un  ejemplo con bgt, void main siempre sirve para meter ahí dentro el código principal, con todo y sus funciones. el uso de esa función siempre será el mismo, mostrar el programa al usuario.

un ejemplo de función sin argumentos puede ser:

```python

def funcion-sin-argumentos():
    print("esta es una función sin argumentos")



esta función siempre mostrará un print igual, amenos que dentro del mismo código tu vallas ycambies el mensage de ese print. sinembargo, estas se usan más con fin ordenativo, como para guardar cada cosa en su lugar, como si fueran baldas de un mismo armario u ojas de un mismo archivador.

#####funciones con argumentos:
estas vienen a ser como vísteis en el primer ejemplo, funciones que sirven para que el programador las use para algo, o para que el usuario cargue algo. por ejemplo, una función para carga del usuario sería input(), que sirve  para introducir texto por teclado. también sirven para acortar las líneas de código o resumir líneas que sirven para varios propósitos en un solo argumento.  por ejemplo:

```python

def print-message(message)
    print(message)

si, se que no es la mejor forma de ejemplificar esto. es usar una función con argumentos dentro de una función con argumentos, y huviera salido más  sencillo poner de ejemplo el propio print, pero para que la gente se haga una idea, sirve perfectamente.

ahora, veamos vuestro probable gran enemigo. las listas.


####listas: tu amigo cuando lo conoces, tu enemigo al aprenderlo.

imagina que tienes que guardar muchos datos, o guardar datos diferentes en un solo lugar, o incluso poder recorrer (listar) varios datos en pantalla. una forma de hacerlo sería con variables. varían, y sería una idea poder modificar las variables para cada objeto, pero eso serviría para hacer condicional tras condicional, listando cada variable, y si te enseñara eso ahora mismo estarías vastante enfadado conmigo por darte un tutorial lleno de código basura, además de que me ganaría unas críticas muy bien fundamentadas de todos los programadores que tenemos por aquí.

una lista, sirve para aorrarte ese trabajo, guardar datos en ella (aunque no los tengas y sean datos del usuario), recorrer esos datos con un bucle (en otro cap) y demás cosas.

una lista vacía se ve así:

```python

lista=[]

eso es una lista, y todo el contenido que le metas dentro está entre esos corchetes. para simplificarlo, imagínate que si las variables son unas cestas donde guardar cosas, las listas son unos camiones de cosas, donde puedes guardar de todo tipo y en mucha cantidad.

y llegados a este punto, entiendo que te preguntes. bale, todo bién. guardo cosas en las listas, pero ¿luego, como las uso? ¿tengo que mencionar toda la lista, hacer que mi usuario se trague las 2000 cosas que tengo ahí hasta llegar a la que le interese?


pues... si. no, es broma. una vez guardes elementos en la lista, todos tienen su índice. es decir, un número que se les asigna, por que están en cila, y cada quien tiene un número para ser llamado. los números, a diferencia de bgt, empiezan desde 0, siendo 0 el primero, y hasta el último correspondiendo cuantas cosas metiste en la lista. por ejemplo, si metiste 4 cosas, el último sería el número 3.

ahora, veamos una lista con cosas.

```python

lista=["manzanas", "peras", "aguacates", "limones"]

print(lista[0]) #el output que recivirás al ejecutar esto, será manzanas



hasta aquí todo bién, lógico deecho. pero hay algo extraño, algo que no vísteis antes. después del print, hay una línea extraña, ¿no? algo que empieza con un # (signo de número, alt derecho mas 3) y después es un texto.
como pudísteis ver, el output es manzanas, por que hice referencia a imprimir el primer elemento de la lista (lista[0])

así será con todos los elementos que quieras imprimir.

ahora, vallamos con nuestro último aprendizage de hoy. los comentarios

####comentarios

los comentarios, son a la vez, la mas insignificante cosa que aprenderás y una de las más importantes.

comentar un código es lo que te permitirá señalar partes que no funcionan bién, pedazos de código que no quieres quitar por que arreglarás, pero tampoco necesitas que estén en el código por que arrojan errores o son innecesarios, o deben ser optimizados de mejor manera, indicar nombres de variables, explicar como funciona el código para permitirles a otros programadores entenderlo mejor, dando igual como lo escribas... por ejemplo, voy a poner un código algo más complicado, con y sin comentarios, haver cuando lo entendéis mejor.

```python

import random

rand=random.randint(1, 9)

if num==8:
    print(el número es 8)

else:
    print("el número no es 8")



como veis, hay conceptos que no hemos explorado por ahora, y que probablemente no entenderéis casi en nada si no dominais un poco el inglés o si veniis de 0 con la programación. un programador que más o menos sepa de esto aunque no sepa python entenderá, por que el código  es claro y se puede interpretar bién. pero un beginer, quizá tenga algunos problemas con el. ahora, hagamos el mismo código pero comentado.
```python

#importamos el módulo random para generar números aleatorios
import random
#declaramos una variable rand, donde inicializamos el objeto randint de random, para generar un número aleatorio entre 1 y 9
rand=random.randint(1, 9)
# verificamos si el número es 8 o no. si lo es, mostramos un mensaje en pantalla
if num==8:
    print(el número es 8)

else:
    #si el número no es 8, mostramos otro mensage
    print("el número no es 8")

¿lo ves? ¡mucho más comprensible!

hay 2 tipos de comentarios. los comentarios de una sola línea y los multilineales.

los de una sola línea son los que ya vimos, están en este código y en el de las listas. se inicializan con un signo de número (#) y la línea que comentes de esa manera no será interpretada por el motor python, simplemente será ignorada igual que ella me ignora... dadme un segundo, tengo que ir a llorar.


listo, volví. siguiendo con el tema comentarios... ejem, ejem. ¿que me miras así? no, no fui a llorar, obvio. ah, ya déjame, tengo que acabar esta clase.


bien, ahora los comentarios multi lineales. estos se declaran con 3 comillas dobles (") y se cierran de la misma manera. un ejemplo de comentario sería:

"""esto es un comentario multilineal.


puedo escribir 9 biblias aquí, y no pasaría nada.
"""

###tareas:

y ahora, ¡las venditas tareas!

**veamos:**

- 1. crea una lista de 5 elementos, e imprime cada uno de ellos.
- 2. crea una función para saludar, una función para despedirse y luego ejecuta las 2 funciones en la parte principal. se hace tal que así.

```python

def saludar():
    print("hola")

def despedirse():
    print("adiós")

saludar()
despedirse()

- 3. comenta esos dos código, explicando cada cosa que haces, y usa un comentario multilineal para explicar el propósito general del programa antes de declarar el código.
