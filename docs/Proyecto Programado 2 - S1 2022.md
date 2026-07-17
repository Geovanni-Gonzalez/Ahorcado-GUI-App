

Ingeniería en Computación
Taller de Programación
## Semestre 1, 2022
## Profesor: Ing. Cristian Campos Agüero

## Proyecto Programado #2
Ahorcado versión Gráfica

## Contenido
-  Introducción ................................................................................................................................ 3
-  Software por desarrollar ............................................................................................................. 3
-  Opciones Administrativas ............................................................................................................ 3
3.1.  Gestión de Palabras ................................................................................................................. 4
3.2.  Gestión de Frases .................................................................................................................... 4
-  Opciones del jugador .................................................................................................................. 5
4.1.  Nuevo Juego ............................................................................................................................ 5
4.2.  Historia del Juego .................................................................................................................... 6
4.3.  Estadísticas de Juegos ............................................................................................................. 7
4.4.  Ayuda....................................................................................................................................... 7
-  Salir .............................................................................................................................................. 8
-  Funciones adicionales ................................................................................................................. 8
-  Aspectos técnicos ........................................................................................................................ 8
-  Documentación ........................................................................................................................... 9
-  Evaluación ................................................................................................................................... 9
-   Forma de trabajo ................................................................................................................... 10
-   Aspectos administrativos ...................................................................................................... 10
-   Rúbrica de evaluación ........................................................................................................... 10
-   Entrega .................................................................................................................................. 11



Índice de Figuras

Figura 1 Pantalla inicio ........................................................................................................................ 3
Figura 2 Menú administrativo ............................................................................................................. 3
Figura 3 Gestión de palabras ............................................................................................................... 4
Figura 4 Gestión de frases ................................................................................................................... 5
Figura 5 Pantalla de jugador................................................................................................................ 6
Figura 6 Ventana de historia del juego ............................................................................................... 6
Figura 7 Estadísticas ............................................................................................................................ 7
Figura 8 Ventana de ayuda .................................................................................................................. 8



## 1. Introducción
Es uno de los juegos de mayor dominio o conocimiento de muchas personas, en la cual consiste en
adivinar una palabra o frase, la persona quien adivina tiene una serie de intentos finitos (mientras
se dibuja a un ahorcado). Fuente: https://es.wikipedia.org/wiki/Ahorcado_(juego)
- Software por desarrollar
Su trabajo consiste en implementar una aplicación de escritorio para administrar el juego utilizando
el lenguaje Python, y programación Iterativa. A continuación, se muestra la pantalla principal del
juego.

Figura 1 Pantalla inicio

## 3. Opciones Administrativas
Una vez seleccionado este, el usuario deberá ingresar una clave de acceso (debe estar generada y
guardada en un archivo, este debe llamarse Acceso.txt) y una vez digitado correctamente se deben
habilitar las siguientes funcionalidades (Opciones administrativas):

Figura 2 Menú administrativo


3.1. Gestión de Palabras
El sistema debe permitir dar mantenimiento de las palabras, se debe permitir incluir, eliminar o
modificar cada una de ellas, además de mostrarlas. La información que se debe almacenar será:
 Identificador (consecutivo autogenerado)
##  Palabra
No pueden existir palabras iguales de la misma manera identificadores repetidos y no pueden
eliminarse palabras que hayan sido asociados a algún juego.
Debe existir un archivo llamado “Palabras.txt” y el formato interno debe ser de la siguiente forma:
## 1, CASA
## 2, MUNDO
## 3, PUERTA

Para poder modificar o eliminar, debe de hacerse seleccionando el item desde el List

Figura 3 Gestión de palabras

3.2. Gestión de Frases
El sistema debe permitir dar mantenimiento de las frases, se debe permitir incluir, eliminar o
modificar cada una de ellas, además de mostrarlas. La información que se debe almacenar será:
 Identificador (consecutivo autogenerado)
##  Frases
No pueden existir frases iguales de la misma manera identificadores repetidos y no pueden
eliminarse frases que hayan sido asociados a algún juego.
Debe existir un archivo llamado “Frases.txt” y el formato interno debe ser de la siguiente forma:

## 1, CASA VERDE
## 2, PLANETA TIERRA
## 3, HOLA MUNDO

Para poder modificar o eliminar, debe de hacerse seleccionando el item desde el List

Figura 4 Gestión de frases

- Opciones del jugador
## 4.1. Nuevo Juego
Una vez seleccionado, con ayuda de los widgets correctos, solicitar el nombre del usuario, obtenido
este, seleccionar el modo de jugo: (Principiante o Avanzado) combo box.
 Si selecciona Principiante, seleccionará al azar una palabra del archivo “Palabras.txt”
 Si selecciona Avanzado, seleccionará al azar una frase del archivo “Frases.txt”
Obtenido estos dos datos, se procede a jugar. Se debe pintar en pantalla los datos como el nombre
del jugador, la palabra o frase, el número de intentos, la lista de letras usadas, el resultado y al
ahorcado.


Figura 5 Pantalla de jugador


Finalizado el juego, se guardará en un archivo llamado “Juego.txt” los siguientes datos bajo el
siguiente formato:
Código, Nombre del jugador, modo, Palabra o frase, total intentos, lista de letras usadas,
resultado, fecha, hora y la duración del juego (NUEVO)
Por ejemplo:
1, Cristian, Principiante, tecnologico, 8, [“A”, “I”, “T”, “N”, “E”, “O”,”C”,”L”],ganador,
12/05/2022, 02:50 pm, 00:02:15
2, Carlo, Principiante, casa, 5, [“D”,”F”,”G”,”H”,”J”], perdió, 12/05/2022, 08:50 am, 00:07:15
4.2. Historia del Juego
En esta opción, se mostrará en pantalla la historia de cómo se creo este juego, la información debe
cargarse desde un archivo llamado “Historia.txt”, el contenido de este lo pueden encontrar como
en Wikipedia u otros sitios en la internet.
Figura 6 Ventana de historia del juego


4.3. Estadísticas de Juegos
Se mostrará los siguientes datos:
- La palabra con el total de derrotas al jugador
- La frase con el total de derrotas al jugador
- El total de juegos a nivel general
- El total de juegos a nivel principiante
- El total de juegos a nivel avanzado
- El total general de juegos ganados y perdidos

Debe estar guardado este dato en un archivo llamado “Estadísticas.txt”.

## Figura 7 Estadísticas

## 4.4. Ayuda
En esta opción, de la misma forma que la sección 4.2, mostrará una explicación al usuario de cómo
jugar este juego. El archivo donde se guardará esta información se llamará “Ayuda.txt”


Figura 8 Ventana de ayuda

## 5. Salir
Finaliza el juego
- Funciones adicionales
 5 puntos adicionales, es decir si las opciones anteriores fueron desarrolladas con éxito. Esta
nueva funcionalidad consistirá en el manejo en dos idiomas, inglés y español. En el
momento de crear un nuevo juego, se le solicitará al usuario en qué idioma será la palabra
para buscar y que además toda la interfaz del juego también esté en inglés
 10 puntos adicionales si en la ventana de Estadísticas muestran los datos en forma gráfica:
o https://www.tutorialesprogramacionya.com/pythonya/detalleconcepto.php?punt
o=73&codigo=73&inicio=60
o https://datapeaker.com/big-data/como-construir-un-pronostico-en-excel
- Aspectos técnicos
El proyecto deberá estar escrito en el lenguaje de programación Python. En caso de requerir librerías
adicionales para compilar y ejecutar el programa, deberán especificarlo en la documentación, ya
que de lo contrario se descontarán puntos en la evaluación. Al iniciar el programa se carga la
información de disco y al salir se guarda (o una la manera permita que todos los datos registrados
sean persistentes).
Y considerar lo siguiente:
 Se debe utilizar iteración en el desarrollo del proyecto, se permiten estructuras como
while y for.
 Se deben manejar mensajes claros al usuario (Messagebox).

 Realizar validaciones de captura de campos. Deben hacer uso de mecanismos de
validación eficientes y mostrarlos con mensajes claros al usuario (Messagebox).
 Número de código o identificador es único y autogenerado
 Toda función bult-in de Python que deseen utilizar debe ser validada con el profesor. Las
funciones eval, append, Split, pop, len no están permitidas.
 El proyecto debe ser guardado en el repositorio del GitHub:
o Taller Grupo 60: https://classroom.github.com/a/GiT2XRs8
o Taller Grupo 61: https://classroom.github.com/a/tcUSRpglv
## 8. Documentación
La documentación es un aspecto de gran importancia en el desarrollo de programas, especialmente
en tareas relacionadas con el mantenimiento de estos.
Para la documentación interna, deberán incluir comentarios descriptivos para cada función, con sus
entradas, salidas, restricciones y objetivo.

La documentación externa deberá incluir:
## 1. Portada.
- Manual de usuario: instrucciones de compilación, ejecución y uso.
- Pruebas de funcionalidad: (Youtube)
- Descripción del problema.
- Diseño del programa: decisiones de desarrollo, algoritmos usados.
- Librerías usadas: creación de archivos, etc.
- Análisis de resultados: lista detallada de objetivos alcanzados, objetivos no alcanzados, y
razones por las cuales no se alcanzaron los objetivos (en caso de haberlos).
- Bitácora (autogenerada, por ejemplo, en GitHub con commit por usuario incluyendo
comentario). Al menos 6 commits
## 9. Conclusión (es)
## 9. Evaluación
La evaluación se va a centrar en dos elementos: programación y documentación. El proyecto
programado tiene un valor de 15% de la nota final, en el rubro de Proyectos.  El desglose de la
evaluación del proyecto programado:
- Documentación interna 4 ptos.
- Documentación externa 6 ptos.
- Funcionalidad 75 ptos (ver detalle en Software a Desarrollar)
- Revisión del proyecto (según completitud del proyecto) 10 ptos.
- Hora de Entrega 5 ptos.

- Forma de trabajo
El trabajo se debe realizar de forma individual o en parejas.
- Aspectos administrativos
Existen 2 carpetas llamadas documentación y programa, en la primera deberá incluir el documento
PDF solicitado y en la segunda los archivos y/o carpetas necesarias para la implementación de este
proyecto programado.  Además, en el archivo llamado README.md, este archivo debe contener la
siguiente información:
a. Nombre del curso
b. Número de semestre y año lectivo
c. Nombre del Estudiante o estudiantes
d. Estatus de la entrega (debe ser CONGRUENTE con la solución entregada):
[Deplorable|Regular|Buena|MuyBuena|Excelente|Superior]
Con este enlace https://docs.github.com/es/github/writing-on-github/getting-started-with-
writing-and-formatting-on-github/basic-writing-and-formatting-syntax le ayudará a dar formato al
archivo README.md
- Rúbrica de evaluación
## FUNCIONALIDAD 75% 0

## Rubro Valor  Obtenido Observaciones
## Opciones Administrativas
Control de acceso 10
Gestión de palabras 15
Gestión de frases 15
Opciones de Jugador
## Nuevo Jugo 10
## Jugar 20
## Historia 5
## Estadísticas 20
## Ayuda 5
## Extras
Manejo de idioma 5
Estadísticas gráficas 10
## TOTAL 115    0
## DOCUMENTACIÓN INTERNA 4%

## DOCUMENTACIÓN EXTERNA 6%

## REVISIÓN DEL PROYECTO 10%

## HORA DE ENTREGA 5%


## NOTA FINAL 100% 0%


## 13. Entrega
En el rubro de “Hora de Entrega” valdrá 5 puntos de la nota total del proyecto, según la siguiente
escala:
a. Si se entrega antes de las 11:55:55 PM del lunes 30 de mayo de 2022, 5 puntos.
b. Si se entrega antes de las 11:55:55 AM el 31 de mayo de 2021, 2.5 puntos.
c. Si se entrega antes de las 11:00:00 PM el 31 de mayo de 2021, 0 puntos.
Después de este punto, NO SE ACEPTARÁN más trabajos.

Todo el contenido de cada proyecto debe ser 100% original y en caso de plagio se asignará nota
cero.