# DOCUMENTACION DE GO #

- [DOCUMENTACION DE GO](#documentacion-de-go)
  - [¿Que es un lenguaje de Programacion?](#que-es-un-lenguaje-de-programacion)
  - [Los lenguajes pueden ser:](#los-lenguajes-pueden-ser)
  - [Origenes del lenguaje Go](#origenes-del-lenguaje-go)
  - [Creadores de Go](#creadores-de-go)
  - [¿Que es Go?](#que-es-go)
  - [¿Porque Go?](#porque-go)
  - [¿Quienes utilizan Go?](#quienes-utilizan-go)
  - [¿Para que sirve Go?](#para-que-sirve-go)
  - [¿Donde encontrar más información?](#donde-encontrar-más-información)
    - [Tutoriales seleccionados:](#tutoriales-seleccionados)
    - [Viajes de aprendizaje guiados:](#viajes-de-aprendizaje-guiados)
    - [Qwiklabs:](#qwiklabs)
    - [Tutoriales:](#tutoriales)
    - [Capacitación:](#capacitación)
    - [Libros:](#libros)
    - [Otras plataformas](#otras-plataformas)
  - [Diferencias entre Nodejs o Java con Go](#diferencias-entre-nodejs-o-java-con-go)
    - [Go vs java y nodejs en términos de concurrencia](#go-vs-java-y-nodejs-en-términos-de-concurrencia)
    - [Go vs nodejs performance en comparación.](#go-vs-nodejs-performance-en-comparación)
    - [Go vs nodejs benchmark en comparación.](#go-vs-nodejs-benchmark-en-comparación)
    - [Go vs nodejs speed en comparación](#go-vs-nodejs-speed-en-comparación)
  - [Instalaciones](#instalaciones)
    - [¿Como se instala Go en Linux?](#como-se-instala-go-en-linux)
    - [¿Como se instala Go en Windows?](#como-se-instala-go-en-windows)
  - [Instalaciones necesarias](#instalaciones-necesarias)
  - [¿Que es Visual Studio Code](#que-es-visual-studio-code)
  - [¿Que es XAMPP?](#que-es-xampp)
  - [Playground de Go](#playground-de-go)
  - [¿Como sabemos que tenemos instalados GO?](#como-sabemos-que-tenemos-instalados-go)
  - [Configurando el entorno de trabajo](#configurando-el-entorno-de-trabajo)
  - [Editor Visual Studio Code](#editor-visual-studio-code)
  - [Extensiones Recomendadas en Visual Studio Code](#extensiones-recomendadas-en-visual-studio-code)
  - [Otros Editores de Código](#otros-editores-de-código)
  - [GoLand](#goland)
  - [Sublime Text](#sublime-text)
  - [Emacs](#emacs)
  - [Vim](#vim)
  - [Sintaxis de Golang](#sintaxis-de-golang)
- [**Declaración de Variables**](#declaración-de-variables)
- [**Inicializacion y Declaracion de variables**](#inicializacion-y-declaracion-de-variables)
  - [Estructuras de control en Go](#estructuras-de-control-en-go)
  - [Bucles](#bucles)


## ¿Que es un lenguaje de Programacion?
Un lenguaje de programación es un lenguaje con reglas gramaticales bien definidas, que proporciona a una persona, en este caso el programador, la capacidad y habilidad de escribir (o programar) una serie de instrucciones o secuencias de órdenes en forma de algoritmos con el fin de controlar el comportamiento de un sistema informático. 

Los lenguajes pueden ser:
----------
- _Interpretados_: ejecutan línea por línea el programa y a la vez ejecutan cada comando.

- _Compilados_: son convertidos directamente a código máquina que el procesador puede ejecutar.
  
- _De alto nivel_: más cerca de la comprensión humana que del código máquina.
  
- _De bajo nivel_: más cerca del código máquina que del lenguaje humano.
  
- _Fuertemente tipados_: exigen que se declare el tipo de dato en las variables, estructura de datos o funciones.
  
- _Debilmente tipados_: no necesitan declarar el tipo de dato, sino que el intérprete (o el compilador) lo deduce.

- _De propósito general_: pueden ser usados para varios propósitos, acceso a bases de datos, comunicación entre computadoras, comunicación entre dispositivos, captura de datos, cálculos matemáticos, diseño de imágenes o páginas.
  
- _De propósito específico_: pueden ser usados para un sólo propósito.
  
Al estudio de los lenguajes en cuanto al enfoque del proceso de programación se le denomina paradigmas de la programación, entendiéndose el término paradigma como la forma de ver y hacer los programas. Bajo este enfoque se tienen cuatro paradigmas los cuales son:

- _paradigma por procedimientos o paradigma imperativo_:
   El paradigma por procedimientos, es tal vez el más conocido y utilizado en el proceso de programación, donde los programas se desarrollan a través de procedimientos. Pascal C y BASIC son tres de los lenguajes imperativos más importantes. La palabra latina imperare significa "dar instrucciones". El paradigma se inició al principio del año 1950 cuando los diseñadores reconocieron que las variables y los comandos o instrucciones de asignación constituían una simple pero útil abstracción del acceso a memoria y actualización del conjunto de instrucciones máquina. Debido a la estrecha relación con la arquitectura de la máquina, los lenguajes de programación imperativa pueden ser implementados muy eficientemente, al menos en principio.

    El paradigma imperativo aún tiene cierto dominio en la actualidad. Una buena parte del software actual ha sido desarrollado y escrito en lenguajes imperativos. La gran mayoría de programadores profesionales son principalmente o exclusivamente programadores imperativos (Hay que añadir que los paradigmas de la programación concurrente y orientada al objeto son en realidad sub-paradigmas de la programación imperativa, así que sus adeptos también son programadores imperativos).

- _paradigma declarativo_: El paradigma declarativo o paradigma de programación lógica se basa en el hecho que un programa implementa una relación antes que una correspondencia. Debido a que las relaciones son mas generales que las correspondencias (identificador - dirección de memoria), la programación lógica es potencialmente de más alto nivel que la programación funcional o la imperativa. El lenguaje más popular enmarcado dentro de este paradigma es el lenguaje PROLOG. El auge del paradigma declarativo se debe a que el área de la lógica formal de las matemáticas ofrece un sencillo algoritmo de resolución de problemas adecuado para, usarse en un sistema de programación declarativo de propósito general.

- _paradigma funcional_: Si la programación imperativa se caracteriza por el uso de variables, comandos y procedimientos, la programación funcional se caracteriza por el uso de expresiones y funciones. Un programa dentro del paradigma funcional, es una función o un grupo de funciones compuestas por funciones más simples estableciéndose que una función puede llamar a otra, o el resultado de una función puede ser usado como argumento de otra función. El lenguaje por excelencia ubicado dentro de este paradigma es el LISP. Por ejemplo si se desea obtener la nota promedio de un alumno podría construirse una función promedio la cual se obtendría a partir de otras funciones más simples: una (sumar) la cual obtiene la suma de las entradas de la lista, otra (contar) la cual cuenta el número de entradas de la lista y la tercera (dividir) que obtiene el cociente de los valores anteriores, su sintaxis será:

    (dividir (sumar notas) (contar notas))

    Obsérvese que la estructura anidada refleja el hecho de que la función dividir actúa sobre los resultados de suma y contar.

- _paradigma orientado a objetos_: El paradigma orientado a objetos, se basa en los conceptos de objetos y clases de objetos. Un objeto es una variable equipada con un conjunto de operaciones que le pertenecen o están definidas para ellos. El paradigma orientado a objetos actualmente es el paradigma más popular y día a día los programadores, estudiantes y profesionales tratan de tomar algún curso que tenga que ver con este paradigma, podría decirse, que programar orientado a objetos está de moda.


[Referencia en wikipedia](https://es.wikipedia.org/wiki/Lenguaje_de_programaci%C3%B3n)

[Referencia en sisbib](https://sisbib.unmsm.edu.pe/bibvirtual/publicaciones/indata/v04_n1/lenguajes.htm)

## Origenes del lenguaje Go

¿Que pasaría si se juntara lo mejor de los lenguajes de Programación [*C*](https://en.wikipedia.org/wiki/C_(programming_language)) y [*Python?*](https://en.wikipedia.org/wiki/Python_(programming_language))  

Eso es lo que pensaron tres programadores de [**Google:**](https://en.wikipedia.org/wiki/Google) 
- [**_Robert Griesemer,_**](https://en.wikipedia.org/wiki/Robert_Griesemer) 
- [**_Rob Pike,_**](https://en.wikipedia.org/wiki/Rob_Pike)
- [**_y Ken Thompson._**](https://en.wikipedia.org/wiki/Ken_Thompson)  
  al sentar las bases para crear en **2009** el lenguaje de programación [*Go.*](https://en.wikipedia.org/wiki/Go_(programming_language))

[**Python**](https://en.wikipedia.org/wiki/Python_(programming_language))  
 es un lenguaje de programación de alto nivel, interpretado, cuya filosofía hace hincapié en la legibilidad de su código, se utiliza para desarrollar aplicaciones de todo tipo, por ejemplo: Instagram, Netflix, Spotify, Panda3D, entre otros. 

*Ejemplo de Python*
```int factorial(int x)
{
    if (x < 0 || x % 1 != 0) {
        printf("x debe ser un numero entero mayor o igual a 0");
        return -1; // Error
    }
    if (x == 0) {
        return 1;
    }
    return x * factorial(x - 1);
}
```
[Referencia en wikipedia](https://es.wikipedia.org/wiki/Python)

 [**C**](https://en.wikipedia.org/wiki/C_(programming_language))  
  es un lenguaje de programación, originalmente desarrollado por [**Dennis Ritchie**](https://en.wikipedia.org/wiki/Dennis_Ritchie) entre 1969 y 1972,​ como evolución del anterior lenguaje B.

 es un lenguaje orientado a la implementación de sistemas operativos, concretamente [*Unix.*](https://en.wikipedia.org/wiki/Unix)  

 C es apreciado por la eficiencia del código que produce y es el lenguaje de programación más popular para crear softwares de sistemas y aplicaciones.

*Ejemplo de C*
```
#include <stdio.h>

int main() {
    int numero;
    fputs("Introduzca un numero entero par: ", stdout);

    if (scanf("%d", &numero) != 1) {
        fputs("Error: numero no valido.\n", stderr);
        return -1;
    }

    for (int i = 2
; numero % 2 == 0; ++i) {
        printf("%.3d| %d/2 = ", i, numero);
        numero /= 2;
        printf("%d\n", numero);
    }

    printf("No se puede seguir dividiendo: El numero %d es impar.\n", numero);
    getchar();

    return 0;
}
```
[Referencia en wikipedia](https://es.wikipedia.org/wiki/C_(lenguaje_de_programaci%C3%B3n))

 ## Creadores de Go ##
- [*Robert Griesemer:*](https://en.wikipedia.org/wiki/Robert_Griesemer) (nacido en 1964) es un informático suizo . Es mejor conocido por su trabajo en el lenguaje de programación [*Go*](https://go.dev/) . Antes de Go, trabajó en el [*motor JavaScript V8 de Google*](https://es.wikipedia.org/wiki/V8_(int%C3%A9rprete_de_JavaScript)) , el lenguaje [*Sawzall*](https://es.wikipedia.org/wiki/Sawzall) , la máquina virtual [*Java*](https://es.wikipedia.org/wiki/Java_(lenguaje_de_programaci%C3%B3n)) [*HotSpot*](https://es.wikipedia.org/wiki/Hotspot_(telecomunicaciones)) y el sistema [*Strongtalk*](https://en.wikipedia.org/wiki/Strongtalk) 

- [*Rob Pike:*](https://en.wikipedia.org/wiki/Rob_Pike) Es mejor conocido por su trabajo en el lenguaje de programación [*Go*](https://en.wikipedia.org/wiki/Go_(programming_language)) y, anteriormente, en los [*Laboratorios Bell*](https://en.wikipedia.org/wiki/Bell_Labs) donde fue miembro del equipo de [*Unix*](https://en.wikipedia.org/wiki/Unix) y participó en la creación del [*Plan 9 de los sistemas operativos Bell Labs*](https://en.wikipedia.org/wiki/Plan_9_from_Bell_Labs)  e [*Inferno*](https://en.wikipedia.org/wiki/Inferno_(operating_system)) , así como el [*lenguaje de programación Limbo.*](https://en.wikipedia.org/wiki/Limbo_(programming_language))

    Pike, junto con [*Ken Thompson*](https://en.wikipedia.org/wiki/Ken_Thompson) es el cocreador de [*UTF-8.*](https://en.wikipedia.org/wiki/UTF-8) Pike también desarrolló sistemas menores, como el programa [*vismon*](https://en.wikipedia.org/wiki/Vismon) para mostrar las caras de los autores de correos electrónicos.

- [*Ken Thompson:*](https://en.wikipedia.org/wiki/Ken_Thompson) Kenneth Lane Thompson (nacido el 4 de febrero de 1943) es un pionero estadounidense de la [*informática.*](https://en.wikipedia.org/wiki/Computer_science) Thompson trabajó en [*Bell Labs*](https://en.wikipedia.org/wiki/Bell_Labs) durante la mayor parte de su carrera, donde diseñó e implementó el sistema operativo [*Unix*](https://en.wikipedia.org/wiki/Unix) original. También inventó el [*lenguaje de programación B,*](https://en.wikipedia.org/wiki/B_(programming_language)) el predecesor directo del [*lenguaje de programación C,*](https://en.wikipedia.org/wiki/C_(programming_language)) y fue uno de los creadores y primeros desarrolladores del sistema operativo [*Plan 9.*](https://en.wikipedia.org/wiki/Plan_9_from_Bell_Labs) Desde 2006, Thompson trabaja en [*Google,*](https://en.wikipedia.org/wiki/Google) donde codesarrolló el lenguaje de programación [*Go.*](https://en.wikipedia.org/wiki/Go_(programming_language))

    Otras contribuciones notables incluyeron su trabajo sobre [*expresiones regulares*](https://en.wikipedia.org/wiki/Regular_expression) y los primeros editores de texto informáticos [*QED*](https://en.wikipedia.org/wiki/QED_(text_editor)) y [*ed*](https://en.wikipedia.org/wiki/Ed_(text_editor)) , la definición de la codificación [*UTF-8*](https://en.wikipedia.org/wiki/UTF-8) y su trabajo sobre ajedrez informático que incluyó la creación de [*tablas de finales*](https://en.wikipedia.org/wiki/Endgame_tablebase) y la máquina de ajedrez [*Belle.*](https://en.wikipedia.org/wiki/Belle_(chess_machine)) Ganó el [*Premio Turing*](https://en.wikipedia.org/wiki/Turing_Award) en 1983 con su colega de muchos años [*Dennis Ritchie.*](https://en.wikipedia.org/wiki/Dennis_Ritchie)
## ¿Que es Go?
Llamado también Golang por su fácil confusión con el verbo Go en Inglés.  
Es un lenguaje de código abierto creado por Google, fue creado para resolver errores internos de la compañia y luego escaló al público general.

Go es un lenguaje de programación compilado, concurrente, imperativo, estructurado y orientado a objetos.

## ¿Porque Go? ##
Es un lenguaje muy seguro debido a su fuerte tipado.  

Go es rápido, eficiente y fácil de usar. 

Go toma ideas de los lenguajes interpretados   para tener una compilación más rápida.

Por ejemplo Go puede estar en Linux y compilar para Windows o viceversa.  
a esto se le llama  
**"Cross-Platform" ó "Cross-Compiled".**

Go demostró ser el lenguaje ideal para grandes desarrollos con miles y miles de usuarios concurrentes y millones de transacciones.

Go fue pensado para aprovechar los últimos avances en hardware, los multiprocesadores, enormes cantidades de memoria y el paralelismo.

Go ahorra en costes y consumo.

Go es fácil de entender, su sintaxis es clara y mejorada con respectos a otros lenguajes.

En Go no hace falta usar puntos y comas.

Las funciones en Go pueden devolver más de un valor.

Solo existe la instrucción FOR para iteraciones 
(No existe while, ni do until, ni nada similar).

Go no es un lenguaje orientado a objetos como tal y resuelve lo que conocemos como POO(Programación Orientada a Objetos) con Estructuras, Funciones, Métodos e Interfaces.

Los métodos y las funciones son lo mismo y los distingue en si devuelve o no un valor(si no los devuelve son métodos).

El Scope(Alcance) de variables, métodos y funciones se determinan con nombres en mayúsculas(para variables globales) y minúsculas(para variables locales).

Es un lenguaje con una gran comunidad de seguidores ya que está respaldado por una gran compañía como Google.

## ¿Quienes utilizan Go? ##

- [**Google**](https://go.dev/solutions/google/)
- [**Paypal**](https://go.dev/solutions/paypal)
- [**American Express**](https://go.dev/solutions/americanexpress)
- [**Mercado libre**](https://go.dev/solutions/mercadolibre)
- [**Bitly**](https://go.dev/solutions/bitly)
- [**Capital one**](https://medium.com/capital-one-tech/a-serverless-and-go-journey-credit-offers-api-74ef1f9fde7f)
- [**Cockroachlabs**](https://www.cockroachlabs.com/blog/why-go-was-the-right-choice-for-cockroachdb/)
- [**Dropbox**](https://dropbox.tech/infrastructure/open-sourcing-our-go-libraries)
- [**Cloudflare**](https://blog.cloudflare.com/graceful-upgrades-in-go/)
- [**Facebook (Meta)**](https://entgo.io/blog/2019/10/03/introducing-ent/)
- [**Microsoft**](https://cloudblogs.microsoft.com/opensource/2018/02/21/go-lang-brian-ketelsen-explains-fast-growth/)
- [**WildLife**](https://medium.com/tech-at-wildlife-studios/pitaya-wildlifes-golang-go-af57865f7a11)
- [**Netflix**](https://netflixtechblog.com/application-data-caching-using-ssds-5bf25df851ef)
- [**Riot games**](https://technology.riotgames.com/news/leveraging-golang-game-development-and-operations)
- [**Salesforce**](https://www.zdnet.com/article/salesforce-why-we-ditched-python-for-googles-go-language-in-einstein-analytics/)
- [**Twitch**](https://blog.twitch.tv/en/2016/07/05/gos-march-to-low-latency-gc-a6fa96f06eb7/)
- [**Twitter (X)**](https://blog.twitter.com/engineering/en_us/a/2015/handling-five-billion-sessions-a-day-in-real-time)
- [**Uber**](https://www.uber.com/en-ES/blog/aresdb/)

## ¿Para que sirve Go? ##
Aunque es un lenguaje multipropósito,  
Se utiliza comúnmente para construir aplicaciones de servidor, herramientas de línea de comandos y aplicaciones de alto rendimiento.

## ¿Donde encontrar más información? ##
Si entramos en la web oficial de [**GO.**](https://go.dev/)  
damos en el botón de [*Get Started*](https://go.dev/learn/) y bajamos la pantalla.  
Tendremos a nuestra disponibilidad los siguientes apartados:

 ### Tutoriales seleccionados: ###
  
¿Eres nuevo en Go y no sabes por dónde empezar?
- [*Documentación:*](https://go.dev/doc/) Todo lo que hay que saber sobre Go.
- [*Tour de Go:*](https://go.dev/tour/welcome/1) Una introducción interactiva a Go con el editor Playground.
- [*Ejemplos:*](https://gobyexample.com/) Una introducción práctica a Go utilizando programas de ejemplos anotados.

 ### Viajes de aprendizaje guiados: ###

 ¿Tienes los conceptos básicos y quieres aprender más?

- [*Desarrollo web:*](https://gowebexamples.com/) cómo utilizar Go para el desarrollo web.
- [*CLI:*](https://spf13.com/presentation/building-an-awesome-cli-app-in-go-oscon/) Taller Creación de una aplicación CLI.
- [*¿Nuevo en la codificación?:*](https://www.youtube.com/watch?v=Q0sKAMal4WQ) Video de Youtube.

### Qwiklabs: ###

Visitas guiadas a los programas de Go.

- [*Implemente aplicaciones Go en plataformas sin servidor de Google Cloud.*](https://www.cloudskillsboost.google/focuses/10532?parent=catalog) 1h 10m 5 Créditos.
- [*Utilice Go Code para trabajar con fuentes de datos de Google Cloud.*](https://www.cloudskillsboost.google/focuses/10531?parent=catalog) 1h 10m 5 Créditos.
- [*Primeros pasos con Go en App Engine.*](https://www.cloudskillsboost.google/focuses/2754?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=5407947) 20m 1 Crédito

### Tutoriales: ###

- [*Empezando*](https://go.dev/doc/tutorial/getting-started) En este tutorial, obtendrá una breve introducción a la programación de Go.
- [*Crear un Módulo*](https://go.dev/doc/tutorial/create-module) un tutorial que presenta algunas características fundamentales del lenguaje Go.
- [*Desarrollando un servicio web*](https://shell.cloud.google.com/?walkthrough_tutorial_url=https%3A%2F%2Fraw.githubusercontent.com%2Fgolang%2Ftour%2Fmaster%2Ftutorial%2Fweb-service-gin.md&pli=1&show=ide&environment_deployment=ide) Este tutorial presenta los conceptos básicos para escribir una API de servicio web RESTful con Go y Gin Web Framework.
  
  ### Capacitación: ###
  Visitas guiadas a los programas de Go.

- [*Laboratorios Ardan:*](https://www.ardanlabs.com/) Ofreciendo clases personalizadas de capacitación en vivo en el sitio.
- [*Guías de Tuza:*](https://www.gopherguides.com/) Clases de formación personalizadas presenciales, remotas y online. Formación para Desarrolladores por Desarrolladores.
- [*Salsa Boss Creativa:*](https://bosssauce.it/services/training) Entrenamiento de Go personalizado o basado en pistas para equipos.
- [*Shiju Varghese*](https://github.com/shijuvar/gokit/tree/master/training) Formación presencial sobre Go y consultoría sobre arquitecturas de sistemas distribuidos, en India.

### Libros: ###
- [*The Go programming language*](https://www.gopl.io/)
- [*Get Programming with Go*](https://www.manning.com/books/get-programming-with-go)
- [*Go programming blueprints*](https://github.com/matryer/goblueprints)
- [*Introducing Go*](https://www.oreilly.com/library/view/introducing-go/9781491941997/)
- [*Concurrency in Go*](https://www.oreilly.com/library/view/concurrency-in-go/9781491941294/)

### Otras plataformas ###
- [*Youtube*](https://www.youtube.com/)
- [*Udemy*](https://www.udemy.com/)
- [*Platzi*](https://platzi.com/)
- [*Codigo Facilito*](https://codigofacilito.com/)

## Diferencias entre Nodejs o Java con Go ##
### Go vs java y nodejs en términos de concurrencia ###

En otros lenguajes también existe el concepto de concurrencia o uno similar. Si comparamos golang vs nodejs por ejemplo, nodejs utiliza un loop de eventos para manejar la concurrencia. Java por su parte utiliza tareas o threads. Existen diferentes enfoques para el manejo de varios procesos de forma simultanea.

Go realiza el manejo de rutinas de forma automática. No hay necesidad de que el programador tenga que preocuparse por esto. Además a comparación de lenguajes como Java y sus tareas, las rutinas solo pesan unos kilobytes de memoria. De tal forma que se pueden crear miles de rutinas sin preocuparse por el desbordamiento de la memoria.

Al abstraer todo el manejo de la concurrencia, las rutinas permiten llevar a cabo todo este proceso sin tener que preocuparse por como se ejecuta esto a nivel del sistema operativo.

### Go vs nodejs performance en comparación. ###

Si lo que deseamos es realizar una comparación entre golang vs nodejs en términos de performance, debemos considerar que go es mas potente que nodejs por las siguientes razones.

El performance de Go al ser compilado es mas similar al de lenguajes como de C o C++.

Su administrador de la memoria o garbage colector es de nueva generación, por lo que permite el manejo y el aprovechamiento de esta de mejor forma.

### Go vs nodejs benchmark en comparación. ###
Existen múltiples ejemplos de laboratorio en los cuales se ha realizado una comparativa de benchmark entre golang vs nodejs, los resultados arrojados suelen ser los mismos.  
Go es el indiscutible líder del mercado. Esto debido a que JavaScript requiere ser interpretado por el motor V8 de Nodejs para poder ser ejecutado.

### Go vs nodejs speed en comparación ###
Desde la aparición de Go en el 2009, los desarrolladores han podido construir aplicaciones muy veloces. Nodejs es un lenguaje muy potente en términos de desarrollo de aplicaciones a nivel del backend. 

Permite entre otras realizar tareas complejas en tiempos relativamente cortos.

Por su parte Golang en términos de velocidad es superior pero requiere de un mayor número de líneas para completar una misma tarea.

## Instalaciones ##
### ¿Como se instala Go en Linux? ###
  1. Elimine cualquier instalación anterior de Go eliminando la carpeta /usr/local/go (si existe),  
  2.   luego extraiga el archivo que acaba de descargar en /usr/local, creando un árbol de Go nuevo en /usr/local/go:
    
  ``` 
  $ rm -rf /usr/local/go && tar -C /usr/local -xzf go1.21.5.linux-amd64.tar.gz
  ```
(Es posible que deba ejecutar el comando como root o mediante sudo).

No descomprima el archivo en un árbol /usr/local/go existente. Se sabe que esto produce instalaciones Go rotas.

3. Agregue /usr/local/go/bin a la PATHvariable de entorno.
Puede hacer esto agregando la siguiente línea a su $HOME/.profile o /etc/profile (para una instalación en todo el sistema):

```
export PATH=$PATH:/usr/local/go/bin
```
**Nota**: Es posible que los cambios realizados en un archivo de perfil no se apliquen hasta la próxima vez que inicie sesión en su computadora. Para aplicar los cambios inmediatamente, simplemente ejecute los comandos del shell directamente o ejecútelos desde el perfil usando un comando como source $HOME/.profile.

4. Verifique que haya instalado Go abriendo un símbolo del sistema y escribiendo el siguiente comando:
   
   ```
    $ go version
   ```

5. Confirme que el comando imprima la versión instalada de Go.

[Referencia web oficial Golang](https://go.dev/doc/install)

### ¿Como se instala Go en Windows? ###

1. Abra el instalador de Microsoft que descargó [en la pagina oficial de Go](https://go.dev/dl/) y siga las instrucciones para instalar Go.  
   
De forma predeterminada, el instalador instalará Vaya a Program Files o Program Files (x86). Puede cambiar la ubicación según sea necesario. Después de la instalación, deberá cerrar y volver a abrir cualquier símbolo del sistema abierto para que los cambios en el entorno realizados por el instalador se reflejen en el símbolo del sistema.

2. Verifique que haya instalado Go.
   1. En Windows, haga clic en el menú Inicio .
   2. En el cuadro de búsqueda del menú, escriba cmd y luego presione la tecla Intro .
   3. En la ventana del símbolo del sistema que aparece, escriba el siguiente comando

```
$ go version
```
 Confirme que el comando imprima la versión instalada de Go.
 ## Instalaciones necesarias ##
 1. Visual Studio Code. [*(Editor de codigo.)*](https://desarrolloweb.com/colecciones/editores-codigo)
 2. XAMPP.(Opcional)

## ¿Que es Visual Studio Code ##
[Visual Studio Code](https://code.visualstudio.com/download) es un editor de código perteneciente a la compañía Microsoft, es multiplataforma, gratuito y de código abierto.

## ¿Que es XAMPP? ##
[XAMPP](https://www.apachefriends.org/download.html) es un entorno de desarrollo multiplataforma y opensource con una distribución de Apache fácil de instalar y que contiene MariaDB, PHP y Perl.

- *_Apache_*: es un servidor para alojar por ejemplo páginas webs en el backend.
- *_MariaDB_*: es una base de datos muy similar a sql(lenguaje de consultas estructurados).
- *_Php_*: (acrónimo recursivo de PHP: Hypertext Preprocessor) es un lenguaje de código abierto muy popular especialmente adecuado para el desarrollo web y que puede ser incrustado en HTML.
- Perl: Perl es un lenguaje de programación diseñado por Larry Wall en 1987. Perl toma características del lenguaje C, del lenguaje interpretado bourne shell (sh), AWK, sed, Lisp y, en un grado inferior, de muchos otros lenguajes de programación.

## Playground de Go ##
Se trata de un editor en linea que sirve para probar el código y que está situado en la misma página web oficial de [**GO.**](https://go.dev/play/)   

En el mismo se incluyen los siguientes botones:
- Run: para ejecutar el código.
- Format: para formatear el código.
- Share: para compartir el código.

y un largo presets precargados para seleccionar.

## ¿Como sabemos que tenemos instalados GO?
- Escribimos go en una terminal de nuestro sistema operativo y nos tiene que salir esto:

 ```
C:\Users\Moises Dominguez>go
Go is a tool for managing Go source code.

Usage:

        go <command> [arguments]

The commands are:

        bug         start a bug report
        build       compile packages and dependencies
        clean       remove object files and cached files
        doc         show documentation for package or symbol
        env         print Go environment information
        fix         update packages to use new APIs
        fmt         gofmt (reformat) package sources
        generate    generate Go files by processing source
        get         add dependencies to current module and install them
        install     compile and install packages and dependencies
        list        list packages or modules
        mod         module maintenance
        work        workspace maintenance
        run         compile and run Go program
        test        test packages
        tool        run specified go tool
        version     print Go version
        vet         report likely mistakes in packages

Use "go help <command>" for more information about a command.

Additional help topics:

        buildconstraint build constraints
        buildmode       build modes
        c               calling between Go and C
        cache           build and test caching
        environment     environment variables
        filetype        file types
        go.mod          the go.mod file
        gopath          GOPATH environment variable
        gopath-get      legacy GOPATH go get
        goproxy         module proxy protocol
        importpath      import path syntax
        modules         modules, module versions, and more
        module-get      module-aware go get
        module-auth     module authentication using go.sum
        packages        package lists and patterns
        private         configuration for downloading non-public code
        testflag        testing flags
        testfunc        testing functions
        vcs             controlling version control with GOVCS

Use "go help <topic>" for more information about that topic.

```
## Configurando el entorno de trabajo ##

Para saber donde es el espacio de trabajo de Go, podemos ejecutar el siguiente comando en la terminal

```
$ go env
```
una vez esto, la terminal listará todas las variables de entorno de Go y nos saldrá algo así...
```
C:\Users\Moises Dominguez>go env
set GO111MODULE=
set GOARCH=amd64
set GOBIN=
set GOCACHE=C:\Users\Moises Dominguez\AppData\Local\go-build
set GOENV=C:\Users\Moises Dominguez\AppData\Roaming\go\env
set GOEXE=.exe
set GOEXPERIMENT=
set GOFLAGS=
set GOHOSTARCH=amd64
set GOHOSTOS=windows
set GOINSECURE=
set GOMODCACHE=C:\Users\Moises Dominguez\go\pkg\mod
set GONOPROXY=
set GONOSUMDB=
set GOOS=windows
set GOPATH=C:\Users\Moises Dominguez\go
set GOPRIVATE=
set GOPROXY=https://proxy.golang.org,direct
set GOROOT=C:\Users\Moises Dominguez\go
set GOSUMDB=sum.golang.org
set GOTMPDIR=
set GOTOOLCHAIN=auto
set GOTOOLDIR=C:\Users\Moises Dominguez\go\pkg\tool\windows_amd64
set GOVCS=
set GOVERSION=go1.21.5
set GCCGO=gccgo
set GOAMD64=v1
set AR=ar
set CC=gcc
set CXX=g++
set CGO_ENABLED=0
set GOMOD=NUL
set GOWORK=
set CGO_CFLAGS=-O2 -g
set CGO_CPPFLAGS=
set CGO_CXXFLAGS=-O2 -g
set CGO_FFLAGS=-O2 -g
set CGO_LDFLAGS=-O2 -g
set PKG_CONFIG=pkg-config
set GOGCCFLAGS=-m64 -fno-caret-diagnostics -Qunused-arguments -Wl,--no-gc-sections -fmessage-length=0 -ffile-prefix-map=C:\Users\MOISES~1\AppData\Local\Temp\go-build2340996025=/tmp/go-build -gno-record-gcc-switches
```
De entre todas las variables de entorno listadas nos fijaremos en esta:
```
set GOPATH=C:\Users\Moises Dominguez\go
```
esa será la dirección de trabajo de Go.  
luego tendremos que escribir el siguiente comando para listar las subcarpetas de donde nos encontramos.

```
C:\Users\Moises Dominguez>dir
```

sino la tenemos, tendremos que crearla.

```
C:\Users\Moises Dominguez>mkdir go
```
y movernos hacia ella..

```
C:\Users\Moises Dominguez>cd go
```
si tenemos que ir hacia atrás en la dirección usaremos los dos puntos.

```
C:\Users\Moises Dominguez>cd ..
```

una vez en la carpeta go, nos saldrá la terminal así...

```
C:\Users\Moises Dominguez\go>
```

ahora tenemos que crear la carpeta src, que es en donde tendremos el código fuente, es decir, los programas ó proyectos que nosotros mismos realizaremos.

pero antes volveremos a listar para ver si ya tenemos creada la carpeta src o no en la dirección de go.
```
C:\Users\Moises Dominguez\go>dir
```
y nos saldrá algo así....

```
 Directorio de C:\Users\Moises Dominguez\go

10/12/2023  04:42    <DIR>          .
10/12/2023  04:42    <DIR>          ..
10/12/2023  04:42    <DIR>          api
10/12/2023  04:42    <DIR>          bin
29/11/2023  21:21                52 codereview.cfg
29/11/2023  21:21             1.337 CONTRIBUTING.md
10/12/2023  04:42    <DIR>          doc
10/12/2023  03:34    <DIR>          go
29/11/2023  21:21               505 go.env
10/12/2023  04:41    <DIR>          lib
29/11/2023  21:21             1.479 LICENSE
10/12/2023  04:42    <DIR>          misc
29/11/2023  21:21             1.303 PATENTS
10/12/2023  04:41    <DIR>          pkg
29/11/2023  21:21             1.455 README.md
29/11/2023  21:21               419 SECURITY.md
10/12/2023  19:27    <DIR>          src
10/12/2023  04:42    <DIR>          test
29/11/2023  21:21                35 VERSION
               8 archivos          6.585 bytes
              11 dirs  137.057.599.488 bytes libres
```
en mi caso ya tengo creada la carpeta src.  
si tu no la tienes creada, tendrás que crearla de la siguiente manera...

```
C:\Users\Moises Dominguez\go>mkdir src
```
y luego volveremos a movernos en la terminal, esta vez hacia la carpeta de src...

```
C:\Users\Moises Dominguez\go>cd src
```
ahora te saldrá así la terminal

```
C:\Users\Moises Dominguez\go\src>
```
ahora crearemos una carpeta para meter dentro nuestro primer proyecto, la carpeta tendrá el nombre que nosotros queramos, por ejemplo:

```
C:\Users\Moises Dominguez\go\src>mkdir hola-mundo
```

navegamos hasta nuestra carpeta.

```
C:\Users\Moises Dominguez\go\src>cd hola-mundo
```

la terminal nos quedará así...

```
C:\Users\Moises Dominguez\go\src\hola-mundo>
```
y desde esta dirección abriremos visual studio code.
con el siguiente comando.
```
C:\Users\Moises Dominguez\go\src\hola-mundo>code .
```

## Editor Visual Studio Code ##

Visual Studio Code (VS Code) es uno de los editores de código más populares y versátiles en la actualidad.   

Gracias a su amplia comunidad de extensiones, podemos agregar funcionalidades específicas para programar en Go.

VS Code también ofrece integración con herramientas populares como el administrador de dependencias Go Modules y el formateador de código gofmt.

[Descargar Visual Studio Code](https://code.visualstudio.com/)
## Extensiones Recomendadas en Visual Studio Code #  
Algunas extensiones recomendadas son:

 - **Go:** Ofrece herramientas de auto-completado, sugerencias y soporte para la depuración de código.
 - **Go Test Explorer:** Facilita la ejecución y visualización de pruebas unitarias.
 - **GoDoc:** Proporciona acceso rápido a la documentación de paquetes y funciones.
  
## Otros Editores de Código ##
## GoLand ##
GoLand es un IDE desarrollado específicamente para programar en Go por JetBrains, la misma compañía que creó IntelliJ IDEA. GoLand ofrece una amplia gama de características diseñadas para mejorar la productividad en Go, como:

- **Finalización de código inteligente:** Ayuda a ahorrar tiempo al ofrecer sugerencias y autocompletado de código.
- **Navegación eficiente:** Permite saltar rápidamente entre archivos, funciones y métodos.
- **Soporte para pruebas unitarias:** Facilita la ejecución y visualización de pruebas, así como la generación automática de pruebas.
- **Análisis de código estático:** Ayuda a detectar errores y sugerir mejoras en nuestro código.

GoLand también cuenta con integración directa con herramientas como el formateador de código gofmt, el administrador de dependencias Go Modules y el generador de documentación go doc.

[Descargar GoLand](https://www.jetbrains.com/go/)

## Sublime Text ##

Sublime Text es un editor de código liviano y altamente personalizable.  

Aunque no está específicamente diseñado para Go, podemos aprovechar su flexibilidad y extensibilidad para programar en este lenguaje.  

Sublime Text se caracteriza por su rendimiento rápido y su amplia selección de temas y esquemas de color, lo que permite personalizar la apariencia del editor según nuestras preferencias.

Algunas extensiones útiles para trabajar con Go en Sublime Text son:

- **GoSublime:** Ofrece resaltado de sintaxis, autocompletado y acceso rápido a la documentación de Go.
- **GoBuild:** Facilita la compilación y ejecución de programas Go directamente desde Sublime Text.
- **GoImports:** Ayuda a organizar las importaciones de nuestro código de forma automática.
  
[Descargar Sublime Text](https://www.sublimetext.com/)

## Emacs ##
Emacs es un editor de texto extensible y altamente personalizable. Aunque su curva de aprendizaje puede ser empinada para algunos usuarios, ofrece una gran flexibilidad y potencia para programar en Go.

Algunas extensiones populares para trabajar con Go en Emacs son:

- **go-mode:** Proporciona funciones de autocompletado, resaltado de sintaxis y navegación rápida entre archivos.
- **go-eldoc:** Muestra información contextual sobre los símbolos mientras escribimos código.
- **go-guru:** Ofrece análisis de código avanzado, como encontrar referencias y mostrar el flujo de llamadas.

Emacs también permite personalizar casi todos los aspectos del editor, desde la apariencia hasta los atajos de teclado, lo que lo convierte en una opción popular entre los programadores más experimentados.

## Vim ##
Vim es un editor de texto modal y altamente configurable.  

Aunque su enfoque basado en modos puede resultar intimidante para los principiantes, ofrece una experiencia de edición rápida y eficiente para aquellos que dominan sus funcionalidades.  

Para programar en Go con Vim, podemos utilizar algunas extensiones como:

- **vim-go:** Proporciona un conjunto completo de herramientas y comandos específicos para Go, como la navegación entre archivos, el formateo de código y la ejecución de pruebas.
- **vim-test:** Permite ejecutar y depurar pruebas unitarias desde Vim.
  
Vim se destaca por su velocidad y capacidad de personalización.  
Con una configuración adecuada, se puede adaptar perfectamente a nuestras necesidades de desarrollo en Go.

A la hora de programar en Go, contar con un editor de código adecuado es fundamental para maximizar la eficiencia y disfrutar de una experiencia de desarrollo fluida.   
 
Los editores mencionados anteriormente, como Visual Studio Code, GoLand, Sublime Text, Emacs y Vim, ofrecen características y extensiones específicas que facilitan la escritura de código en Go, como resaltado de sintaxis, autocompletado, herramientas de prueba y navegación rápida entre archivos.   
 
La elección del editor dependerá de nuestras preferencias personales y del flujo de trabajo que mejor se adapte a nuestras necesidades

## Sintaxis de Golang ##

Siempre que empecemos a escribir código en un programa de Golang, tendremos 2 normas de obligatoria sintaxis. 
   
 1. Lo primero será poner en la cabecera del código el package main..  
   (Esto servirá para decirle al código que de todos  este será el paquete principal).

```
package main
```
  2. Lo segundo será poner la función principal para poder meter dentro el código a programar.

```
func main() {
	
}
```

una vez hechos estos dos pasos, estaremos listos para programar, siempre dentro de la función main.

**Hola Mundo en GO**
 ```
 // comentario en linea
/*
    comentario en bloque
*/ 


/* siempre tenemos que poner en que paquete estamos y en el programa principal siempre será el main.
esto servirá para decirle al código que de todos los paquetes este será el principal*/
package main 

/* importamos el paquete standart fmt para poder imprimir por pantalla*/
import "fmt" 

/* funcion principal equivalente al paquete principal, toda aplicación empieza por esta función */
func main() {
    /* con este metodo de la libreria fmt imprimimos por pantalla */
	fmt.Println("Hola, Mundo")
}

 ```
 así nos quedaría el código para escribir nuestro primer Hola Mundo.
 ```
 package main

import "fmt"

func main() {
	fmt.Println("Hola, Mundo")
}

 ```

Es importante saber que la extensión de todo programa en Go es .go

Para ejecutar nuestro programa abriremos un nuevo terminal de visual studio que se abrirá en nuestro directorio.

Terminal > nuevo terminal

```
PS C:\Users\Moises Dominguez\go\src\hola-mundo>
```

escribiremos el siguiente comando en la terminal para ordenarle al código que se ejecute.

```
PS C:\Users\Moises Dominguez\go\src\hola-mundo> go run hola.go
```

"en mi caso el programa se llama hola.go"

```
PS C:\Users\Moises Dominguez\go\src\hola-mundo> go run hola.go  
Hola, Mundo
PS C:\Users\Moises Dominguez\go\src\hola-mundo> 
```
Esto sólo compilará internamente y no creará ningún archivo, para la producir, exportar y compartir nuestro archivo utilizaremos este otro comando.

```
PS C:\Users\Moises Dominguez\go\src\hola-mundo> go build hola.go
```

si listamos en nuestro directorio obtendremos los dos archivos, el interno y el externo.

```
PS C:\Users\Moises Dominguez\go\src\hola-mundo> dir


    Directorio: C:\Users\Moises Dominguez\go\src\hola-mundo    


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/12/2023     21:13        1899520 hola.exe     
-a----        10/12/2023     20:47             79 hola.go      


PS C:\Users\Moises Dominguez\go\src\hola-mundo> 
```

el .go es el interno,  
el .exe es el externo.

para ejecutar el externo escribiremos punto y diagonal más el nombre de nuestro programa sin ninguna extensión.

```
PS C:\Users\Moises Dominguez\go\src\hola-mundo> ./hola
Hello World!
PS C:\Users\Moises Dominguez\go\src\hola-mundo> 
```

**Paquetes de terceros o Paquetes externos**  

Los paquetes externos o de terceros son paquetes que no están incluidos en la librería standard tal y como si que lo está el paquete fmt que hemos visto antes.

Estos paquetes han sido desarrollados y mantenidos por la comunidad de desarrolladores de Go.

Para poder usarlos tenemos que inicializar un manejador de modulos para nuestra aplicación.

Para ello usaremos el siguiente comando en una terminal.

```
C:\Users\Moises Dominguez\Desktop\GOLANG> go mod init main.go
```
Observa que al final debe llevar el nombre y la extensión de nuestra aplicación.

con esta respuesta ya habriamos inicializado el manejador de modulos

```
go: creating new go.mod: module main.go
go: to add module requirements and sums:
        go mod tidy
```

Ahora si hacemos un ls y listamos en nuestra dirección veremos que se ha creado un archivo go.mod

```
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        15/12/2023     19:20             26 go.mod
-a----        10/12/2023      5:19             79 main.go
```

Si entramos en dicho archivo veremos el nombre de nuestro manejador de modulos y la versión de Go.

```
module main.go

go 1.21.5
```
El archivo go.mod es un archivo que se utiliza para definir y gestionar los modulos y las dependencias de nuestro proyecto en go.

Tambien se va a crear un archivo que va a ser go.sum 

Dicho archivo se utiliza para registrar la suma de verificaciones de los modulos y las depencias de nuestro proyecto.

Entonces, ahora vamos a utilizar el paquete quot en nuestro proyecto.

El paquete quot es un paquete de terceros o externo en el lenguaje de programación Go que proporciona una serie de citas famosas como el hola mundo.

Para descargar este paquete de terceros y agregarlo a nuestro proyecto vamos a utilizar el siguiente comando.

```
C:\Users\Moises Dominguez\Desktop\GOLANG> go get rsc.io/quote

```
Observemos que dicho comando incluye la ruta del repositorio o de la descripción del paquete.

Al dar a la tecla Intro descargaremos dicho paquete de terceros y lo añadiremos a nuestro manejador de modulos.

```
C:\Users\Moises Dominguez\Desktop\GOLANG> go get rsc.io/quote
go: downloading rsc.io/quote v1.5.2
go: downloading rsc.io/sampler v1.3.0
go: downloading golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c
go: added golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c
go: added rsc.io/quote v1.5.2
go: added rsc.io/sampler v1.3.0
```
Si verificamos nuestro archivo go.mod veremos a dicho paquete externo  ya agregado a nuestro proyecto, listo para importarlo en nuestro proyecto y poderlo utilizar.

```
module main.go

go 1.21.5

require (
	golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c // indirect
	rsc.io/quote v1.5.2 // indirect
	rsc.io/sampler v1.3.0 // indirect
)

```

Si entramos al archivo go.sum veremos registradas las verificaciones del paquete quote y las dependencias de nuestro proyecto.

```
golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c h1:qgOY6WgZOaTkIIMiVjBQcw93ERBE4m30iBm00nkL0i8=
golang.org/x/text v0.0.0-20170915032832-14c0d48ead0c/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
rsc.io/quote v1.5.2 h1:w5fcysjrx7yqtD/aO+QwRjYZOKnaM9Uh2b40tElTs3Y=
rsc.io/quote v1.5.2/go.mod h1:LzX7hefJvL54yjefDEDHNONDjII0t9xZLPXsUe+TKr0=
rsc.io/sampler v1.3.0 h1:7uVkIFmeBqHfdjD+gZwtXXI+RODJ2Wc4O7MPEh/QiW4=
rsc.io/sampler v1.3.0/go.mod h1:T1hPZKmBbMNahiBKFy5HrXp6adAjACjK9JXDnKaTXpA=
```
Para usar el paquete externo en nuestro paquete solo tendremos que importarlo.

```
package main

import (
	"fmt"
	"rsc.io/quote"
)

func main() {
	fmt.Println(quote.Hello()) // Esto imprime Hola Mundo.
}
```

**Declaración de Variables**  
===============================

**Primera Forma**
```
package main

import (
	"fmt"
)

func main() {

	// Declaracion de variables

	var firstName, lastName string
	var age int

    // Inicilizacion de variables
	firstName = "Moises"
	lastName = "Dominguez"
	age = 44;


	fmt.Println(firstName, lastName, age) 
}
```
**Segunda Forma**
```
package main

import (
	"fmt"
)

func main() {

	// Declaracion de variables

	var (
		firstName, lastName string
		 age int
	) 

    // Inicializacion de variables

	firstName = "Moises"
	lastName = "Dominguez"
	age = 44;


	fmt.Println(firstName, lastName, age) 
}
```
**Inicializacion y Declaracion de variables**
===============================================  
**Primera Forma**
```
package main

import (
	"fmt"
)

func main() {

	// Inicializacion y Declaracion de variables

	var (
		firstName = "Moises"
		lastName = "Dominguez"
		age = 44;
	) 

	fmt.Println(firstName, lastName, age) 
}
```
**Segunda Forma**
```
package main

import (
	"fmt"
)

func main() {

	// Inicializacion y Declaracion de variables

	var firstName, lastName, age = "Moises", "Dominguez", 44
		
	fmt.Println(firstName, lastName, age) 
}
```
**Tercera Forma**
```
package main

import (
	"fmt"
)

func main() {

	// Inicializacion y Declaracion de variables

	firstName, lastName, age := "Moises", "Dominguez", 44
		
	fmt.Println(firstName, lastName, age) 
}
```
Esta es la forma más usada para declarar e inicilizar una variable, aunque para poder usar esta forma se debe meter obligatoriamente dentro de la funcion main y la variable debe de ser nueva e inicializada por primera vez.

Con la palabra reservada var si se permite declarar e inicializar las funciones dentro y fuera de la función main.

**Constantes**  
Las constantes a diferencia de las variables, mantienen siempre un valor y este nunca puede ser cambiado. 

```
package main

import "fmt"

const Pi = 3.1416

func main() {
    fmt.Println("El valor de Pi es:", Pi)
}
```
Si se intenta hacerlo, el compilador mostrará un error.

Si intentamos cambiar el valor de Pi, el compilador nos mostrará un mensaje de *"cannot assign to Pi"*, debido a que las constantes no pueden cambiar su valor después de ser definidas.
## Estructuras de control en Go ##
**Estructuras condicionales**  
**If básico**
```
package main
import "fmt"
func main() {
   encendido := true
   if encendido {
      fmt.Println("Está encendido")
   }
}
```
Notarán que es muy parecido a la sintaxis de C o a la mayoría de los lenguajes inspirados en este, la principal diferencia es que los paréntesis alrededor de la condición no son obligatorios, pero de igual forma comprueba si dicha condición es verdadera y en caso de que así sea, realiza las instrucciones que se encuentran dentro de sus respectivas llaves, en caso contrario las instrucciones son ignoradas, nada raro hasta el momento. 

Bastante útil, pero ¿Que sucede si necesito que se ejecute una instrucción en caso de que a condición resulte falsa?

**If-else**

```
package main
import "fmt"
func main() {
    encendido := false
    if encendido {
        fmt.Println("Está encendido")
    } else {
        fmt.Println("Está apagado")
    }
}
```
Perfecto, la confiable instrucción *else* al rescate. En este caso la condición será evaluada como falsa, las instrucciones dentro del *if* son ignoradas y se ejecutan las del *else*.

Otra caso frecuente es necesitar comprobar más de una condición, fácilmente podrías anidar condicionales (colocar otro *if* dentro del bloque del *else*, por ejemplo), pero dependiendo del caso podría ser mas adecuado simplemente usar la estructura *else-if*, aunque será necesario recurrir a un ejemplo diferente al anterior.

**Else-If**
```
package main
import "fmt"
func main() {
   var edad uint8 = 180
   if edad > 150 {
       fmt.Println("¿Eres inmortal?")
   } else if edad >= 18 {
       fmt.Println("Eres mayor de edad")
   } else {
       fmt.Println("Eres menor de edad")
   }
}
```
Hasta el momento nada fuera de lo común, me parece, ahora veamos algo más propio de **Go**.

**If con declaración corta**

```
package main
import "fmt"
func main() {
   if edad := -5; edad > 150 {
       fmt.Println("¿Eres inmortal?")
   } else if edad >= 18 {
       fmt.Println("Eres mayor de edad")
   } else if edad < 18 && edad > 0 {
       fmt.Println("Eres menor de edad")
   } else {
       fmt.Println("Edad fuera del rango")
   }
}
```
Así es, if permite ejecutar una declaración corta antes de comenzar a evaluar las condiciones, es importante resaltar que el ámbito de esa variable está limitado a la propia estructura condicional, intentar acceder a ella desde fuera generará un error al momento de compilar.

**Switch básico**
Como alternativa a múltiples *else-if* contamos con **switch.**
```
package main
import "fmt"
func main() {
    switch dias := 1; dias {
    case 0:
        fmt.Println("Lunes")
    case 1:
        fmt.Println("Martes")
    case 2:
        fmt.Println("Miercoles")
    case 3:
        fmt.Println("Jueves")
    case 4:
        fmt.Println("Viernes")
    case 5:
        fmt.Println("Sabado")
    case 6:
        fmt.Println("Domingo")
    default:
        fmt.Println("Desconocido")
    }
}
```
**Switch sin condición**
```
package main
import "fmt"
func main() {
    var edad uint8 = 18
    switch {
    case edad >= 150:
        fmt.Println("¿Eres inmortal?")
    case edad >= 18:
        fmt.Println("Eres mayor de edad")
    default:
        fmt.Println("Eres menor de edad")
    }
}
```

Dependiendo de la ocasión es una opción elegante y eficiente, pero en este momento me gustaría resaltar algo, si aún no lo notan, no es necesario utilizar *break* al final de cada caso para evitar que continúe ejecutando los posteriores, genial, pero si necesitas que lo haga, basta con colocar la palabra reservada *fallthrough* al final del caso para que continúe con el siguiente.

## Bucles ##

el único constructor para ciclos en **Go** es *for*

**Ciclo for común**
```
package main
import "fmt"
func main() {
    for i := 0; i < 10; i++ {
        fmt.Println(i)
    }
}
```
No hay mucho que decir, el ciclo for de toda la vida para aquellos que conozcan lenguajes como C, Java, JavaScript, entre otros. Lo único novedoso sería el hecho de que, al igual que con los condicionales, no son necesarios los paréntesis.

**For estilo while**
```
package main
import "fmt"
func main() {
    var i = 0
    for i < 10 {
        fmt.Println(i)
        i++
    }
}
```
*for* es el único constructor de ciclos en Go, pero es bastante flexible.

*For-range*
```
package main
import "fmt"
func main() {
    for indice, letra := range "hola mundo" {
        fmt.Println(indice, string(letra))
    }
}
```
Con esta variación del ciclo for es posible recorrer facilmente colecciones como arreglos, mapas, entre otros.

*For-forever*

```
package main
import "fmt"
func main() {
    for {
        fmt.Println("Hola")
    }
}
```
Y así es como podemos hacer un ciclo infinito intencionalmente.

*Defer*
Ahora uno no tan común. *Defer* permite realizar una declaración que se ejecutará al final de la función, antes del retorno, sin importar en que nivel de la misma fue declarada. Veamos un ejemplo.
```
package main
import "fmt"
func main() {
    // Se imprime al final
    defer fmt.Println("primera")
    // Se imprime después de "Hola mundo"
    defer fmt.Println("segunda")
    fmt.Println("Hola mundo")
}
```

Si se están preguntando que utilidad tiene, es perfecta para cerrar recursos, como archivos y conexiones a bases de datos, en **Go** se acostumbra usar justo debajo de la declaración donde se abre el recurso para no olvidar cerrarlo, sabes que de todas formas se ejecutará al final. 

Otra cosa a tener en cuenta respecto a *defer* es que si hay mas de uno en la función se ejecutarán en el orden inverso en el que fueron declarados.
