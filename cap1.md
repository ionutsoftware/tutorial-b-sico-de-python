
## Capítulo Uno: Instalación de Python. ¿Qué necesito para escribir Python? y un "Hola Mundo".

### Instalación de Python

Para comenzar a codificar grandes programas (o pequeños programas), primero necesitamos instalar nuestro traductor de código. El ordenador no entiende nuestro lenguaje, y es por eso que escribir en el idioma del ordenador sería muy complicado. Imagínate escribir todo con unos y ceros, que es el lenguaje binario, y también el lenguaje de los ordenadores.

En ese caso, sería trabajo de ingenieros especializados escribir código, y por supuesto, este tutorial sería bastante más complicado, porque primero tendría que enseñaros lenguaje binario. Afortunadamente, los lenguajes de programación nos ofrecen una escapada de este gran problema.

Un intérprete nos permite escribir nuestro código siguiendo una sintaxis más humana, y en palabras que podamos (o no) entender, pero que al menos sean eso, palabras. En este caso, debemos instalar nuestro intérprete, que será el de Python.

Para ello, podemos descargarlo desde [aquí](https://www.python.org/ftp/python/3.12.0/python-3.12.0-amd64.exe).

Una vez demos clic, el archivo debería empezar a descargarse automáticamente. Entonces, una vez descargado, debemos ir a nuestra carpeta de descargas y darle enter. Una vez hecho eso, el instalador se abrirá.

En la pantalla que se nos abre, hay varias opciones. La que a nosotros nos interesa concretamente es una casilla que dice "Add Python to PATH".

Marcamos esa casilla, que será muy importante, buscamos el botón "Install Now" y lo presionamos. El intérprete de Python se instalará. Al finalizar la descarga, caeremos en otra ventana. De aquí no nos interesa nada, así que presionaremos "Close".

Una vez hecho esto, Python debería estar ya instalado en nuestro sistema. Yo estoy utilizando actualmente Python 3.11.5, aunque la versión que probablemente instales (si estás leyendo esto ahora) es Python 3.12.0.

En fin, a menos que este tutorial sea demasiado antiguo y lleguemos a Python 4, la sintaxis es igual, quizá cambiando un par de cosas, aunque eso ahora no nos interesa. Así que este tutorial va orientado a Python 3.x.

Bien, ahora volviendo, para verificar si tenemos Python correctamente instalado y añadido al "PATH", debemos abrir una ventana de símbolo del sistema. Para ello, presionamos Windows + R y en la ventana que se nos abre ("Ejecutar diálogo") escribimos "cmd" sin las comillas.

Se nos abrirá el cmd (no me pararé a explicar cómo se usa, asumo que ya tenemos un mínimo conocimiento de ello, pero si no, hay muchos tutoriales de introducción a la consola).

Una vez en el cmd, escribiremos "python --version" (sin las comillas). Lo que deberíamos recibir al hacer eso es algo como "Python 3.11.5" aunque puede ser cualquier número de versión. La cuestión es que nos devuelva la versión de Python.

Una vez nos aseguremos de eso, vamos a ver si tenemos nuestra preciada consola interactiva, que nos ayudará un tanto más adelante. Para eso, en el mismo cmd, escribimos "python" y se nos abrirá el intérprete en tiempo real de Python. No me pararé a explicarlo ahora, lo explicaremos en capítulos superiores.

### ¿Qué se necesita para escribir Python?

Bueno, una vez instalado nuestro traductor, ¿necesitamos el campo de texto para enviarle las órdenes, no?

Para ello, un programador usa un "IDE" (Entorno de Desarrollo Integrado), el cual no deja de ser un editor de textos como podría ser el "Bloc de Notas" o "notepad.exe", pero con algunas funciones adicionales. Algunas opciones son "Visual Studio Code", "Notepad++" o "Eclipse".

Pero, si eres igual que yo y te gusta algo tan simple, sin autocompletado de textos ni nada por el estilo, puedes usar el Bloc de Notas de Windows sin ningún tipo de problemas.

En este tutorial (por ahora) utilizaremos el "notepad.exe" por su simplicidad, porque no involucra una curva de aprendizaje y porque por ahora no necesitaremos que nos autocompleten los códigos para poder aprender en condiciones.

Más adelante, mostraré de forma básica cómo programar con Visual Studio Code (VSCode) y su visualizador de problemas, etc.


###un "hola mundo"


a la ora de programar, como en todos los momentos de nuestra vida, emos de empezar desde 0. y en programación, lo más básico que se puede hacer es imprimir un mensage en la pantalla al usuario.

en según que lenguage, esto puede ser una odisea interesante, donde tendría que hacer una pequeña vista a lo que es una clase, un objeto, un método (tranquilos, eso lo veremos un poquito más tarde en otro capítulo)

afortunadamente python no corre con este problema, y escribir un "hola mundo" en python es tan sencillo que nos ocupará una sola línea, 2 si lo queremos ver a detalle. incluso lo podemos hacer con nuestra consola interactiva, pero vosotros quereis crear vuestro primer programa, y yo quiero que también aprendais lo que es la extensión.py y como ejecutar un programa python, así que... tocará hacer un archivo".py"


para empezar, abramos nuestro campo de texto, es decir, el bloc de notas.

para hacer eso, presiona de nuevo windows mas r (familiarízate con este comando, lo usarás vastante) y escribe "notepad" (sin las comillas)
si todo salió bien, deberías de tener un editor de textos avierto y enblanco, el cual será tu lienzo como programador para que plasmes todos los programas que quieras de ahora en adelante. aquí podras escribir clases, métodos, funciones, pero ahora solo escribirás una línea.


la línea a escribir es:


**print("hola mundo")**

pero ¿que hace este código?

bueno. print, es una función. por ahora no hablaremos mucho de ellas, por que veremos más cosas e inclusive como crear la tuya propia un tanto más tarde, pero una función es una órden que tu le das a tu intérprete, la cual contiene una explicación. es decir, aplicándo esto a la vida real, tu le puedes decir a un amigo "compra" pero ¿que compra? por eso, una función podría ser "compra("pan", "queso", "jamón serrano")".

en este caso, lo que le estamos diciéndo a nuestro intérprete es "imprime". "print" significa  imprimir en inglés, y la finalidad de la función es imprimir un mensage en la pantalla. por lo tanto, le decimos "print", pero ¿que imprime? y lo que imprime es lo que va entre los paréntesis, es decir, un argumento. en este caso, lo que le estamos diciendo a nuestro intérprete python es imprime "hola mundo"


bien, una vez escrita así la línea, guardaremos este archivo. utiliza nombres cortos, tales como ejemplo1, o primer-programa. la extensión con la cual lo deberás de guardar, será ".py" así que tu archivo final debe de estar como "archivo(nombre que prefieras).py"

una vez tengas guardado tu programa, ¡felicidades! este es un primer programa que tu y solo tu has creado. ahora, vamos a... ejecutarlo ¿no?

bueno, para ejecutar un programa en python, necesitamos nuestra terminal. python es un intérprete que al  iniciar, a diferencia de otros lenguages como autoit o bgt, tiene funcionalidades que se ejecutan en la consola. es decir, todos los programas son de consola. más tarde empezaremos a darle repasos a las guis en python, pero para eso necesitamos primero conocer las clases, los métodos, las funciones con uno o más argumentos... en fín, demasiadas cosas.

pero para ejecutar este programa... si, ¡adivinaste! necesitas el cmd. ya te dige que te tendrás que familiarizar con el, por que lo usarás mucho con este (y otros) lenguages.

notarás que si abres el cmd como dige anteriormente, se te abre en la carpeta de tu usuario por defecto. bueno, para llegar a la carpeta donde tu has guardado tu archivo python, tendrás que moverte de ahí.

para eso, puedes usar el comando cd. cd  viene del inglés "change directory" "cambiar directorio (carpeta)" pero para eso, tendrás que indicarle al cmd donde está esa carpeta. osea, imagínate que tienes el archivo python en el disco c, en una carpeta llamada pyfiles


entonces, el  comando quedaría "cd C:\pyfiles". desde ahora, se asumirá que tienes todos los archivos en esa carpeta, para tener rutas más cortas y por cuestiones de practicidad.

otra obción de abrir el cmd directamente desde la carpeta en la que está tu archivo python, es entrar desde la gui de windows en la carpeta, presionar alt mas d y en el campo dirección escribir "cmd".


asumiendo que entraste a la carpeta con el cmd de alguna de las dos maneras, para poder ejecutar tu programa deberás llamar a python, para que sepa que ese programa tiene que ver con el, por que el solito no se da por aludido, es como ese amigo despistado que puedes estar hablando de el y no se daría ni cuenta. para eso lo llamamos. "python" pero claro, si lo llamas te responderá ¿e? ¿que decías? y eso se traduce en que nos abrirá la consolita interactiva,, por que no save que quieres que haga. para eso, escribiremos python, un espacio, y el nombre del archivo (con todo y extensión) para que nuestro traductor sepa que traducir. entonces, y tomando por defecto que tu archivo se llama "example.py", la llamada al intérprete sería "python example.py"

dando enter sobre ese comando, deverás escuchar el siguiente mensage: "hola, mundo". si eso pasa, significa que... ¡urra! tu  primer programa está echo.

si ves algún error, verifica que la línea esté bien copiada.


¡has llegado al final de este primer capítulo! si te ha gustado, dame un +1, y postea para que pueda venir con el capítulo 2, las variables.