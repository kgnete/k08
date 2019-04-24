[README](README.md)

## Instalación VirtualEnv

 Marcar esta página

Una de las grandes fortalezas de Python es que viene con una **multitud de módulos** ya implementados que nos van a permitir desarrollar fácilmente en nuestras aplicaciones.

Es por esto que **instalar bibliotecas** es una de las actividades más comunes que vamos a ejecutar dentro de Python para crear aplicaciones. Sin embargo, nos puede dar problemas porque, como todas las aplicaciones se basan fuertemente en el uso de bibliotecas externas, a veces estos módulos no son compatibles entre sí o podemos necesitar versiones distintas para distintos programas.

VirtualEnv es un entorno que nos va a permitir **aislar la instalación de ciertas bibliotecas** para que solamente las utilicemos con ciertos programas en Python.

### 















0:00 / 0:00

Velocidad: Presiona ARRIBA para acceder al menú, luego usa las teclas de ARRIBA y ABAJO para cambiar a diferentes velocidades, y presiona ENTER para cambiar a la velocidad seleccionada.

Haz clic en este botón para silenciar o activar el sonido del vídeo o usa los botones ARRIBA o ABAJO para aumentar o disminuir el nivel de volumen.

Máximo Volumen.



### Transcripción de video

1. [Inicio de la transcripción. Saltar al final.](https://courses.edx.org/courses/course-v1:UAMx+WebApp+1T2019a/courseware/2062d8c9518447c7b1c6749f85df98df/1c322177492548f79c0c7f363b92bd81/1?activate_block_id=block-v1%3AUAMx%2BWebApp%2B1T2019a%2Btype%40vertical%2Bblock%402783ad7dc6f14b2fb032e39532163f17#transcript-end-82402fc855f54e8195e1f8d6fa0d1117)
2. El siguiente paso es instalar el VirtualEnv con el gestor de paquetes de la distribución de Linux,
3. de Ubuntu en este caso, que como hemos visto antes es “apt”.
4. El siguiente es ejecutar aquí “virtualenv”, dice que no existe y entonces lo único que tengo que hacer es
5. “sudo apt install" y en este caso queremos instalar VirtualEnv.
6. Se conecta a los repositorios, se da cuenta de que estamos trabajando con Python 3,
7. se descarga la versión correcta, y cuando lo ejecutamos lo instala y,
8. si ahora abro un nuevo terminal para ver las modificaciones,
9. tengo instalado VirtualEnv en la máquina.
10. El siguiente paso es configurar y empezar a utilizar VirtualEnv.
11. En lo que se refiere a la configuración, lo único que vamos a hacer es crear un directorio
12. en el que almacenar todos los entornos virtuales. Lo que yo os propongo es un directorio que
13. se llame virtualenvs, que sea un directorio oculto, de ahí que
14. esté el punto (.) delante del directorio y que se encuentren en el home del usuario.
15. Si creamos ese directorio, inicialmente estará vacío.
16. Vamos a crear nuestro primer entorno virtual. Para ello, simplemente tenemos que llamar a virtualenvs,
17. darle la ruta en la que queremos que almacene el entorno virtual y el nombre del entorno virtual,
18. todo como un directorio.
19. Cuando hacemos esto, en lo que se traduce es que ese directorio que antes estaba vacío
20. ahora tiene un nuevo directorio, que se llama web,
21. y que dentro del directorio web existen otra serie de directorios y de ficheros donde están,
22. por ejemplo, dentro del directorio bin, las herramientas para trabajar con VirtualEnv,
23. el pip con el que vamos a trabajar, las versiones de Python,
24. tenemos librerías en las que está, en este caso Python3 y esto se va a empezar a rellenar
25. a medida que trabajemos con el entorno virtual. Otra cosa que podemos hacer, relacionada con
26. la configuración en este caso de pip, pero relacionado con los entornos virtuales,
27. es obligar a que no podamos instalar ni desinstalar ningún módulo de Python si no es dentro
28. de un entorno virtual. ¿Qué es lo que conseguimos con esto?
29. Pues evitar errores, evitar que yo borre accidentalmente un módulo
30. que utiliza una aplicación crítica o que actualice a una nueva versión un módulo
31. que utiliza otra aplicación crítica.
32. Para ello, lo que vamos a utilizar es la variable entorno, PIP_REQUIRE_VIRTUALENV.
33. Si yo esta variable la fijo a true (“export PIP_REQUIRE_VIRTUALENV=true”),
34. lo que estoy haciendo es que pip no pueda instalar ningún módulo si no estás dentro de un entorno virtual.
35. Si yo intento instalar, por ejemplo, el módulo pprint, como he fijado esa variable a true
36. me dice que no puedo trabajar con pip, no se puede instalar,
37. porque no estoy dentro de un entorno virtual de esta forma, como ya decía, evitamos errores.
38. Que quiero, ya porque estoy seguro de ello, instalar o borrar una librería general del sistema,
39. lo único que tengo que hacer es quitar esa variable de entorno (“unset PIP_REQUIRE_VIRTUALENV”).
40. Le quito el valor y ahora intento instalar el módulo pprint, en este caso.
41. Para no tener que hacerlo cada vez, lo que podemos hacer es fijar esa variable de entorno en nuestro bashrc.
42. Aquí, en nuestro bashrc, lo que yo podría hacer es poner esta línea y, cada vez que
43. abriera una sesión con bash, se fijaría y la variable PIP_REQUIRE_VIRTUALENV
44. no tendría que ir fijándola cada vez. Ahora que ya tenemos creado nuestro entorno
45. virtual, el siguiente paso es empezar a trabajar con él.
46. Para ello, lo que tenemos que hacer es llamar a través de source
47. a uno de los ficheritos que ha dejado en el directorio bin, que veíamos antes.
48. Este ficherito es “activate”, que lo que hace es activar ese entorno virtual; en este
49. caso, el entorno virtual “web”.
50. Vemos que ha cambiado la prompt, me ha puesto aquí entre paréntesis el nombre del entorno virtual activo,
51. y eso significa que todo lo que llevaba ahora con Python, ya sea invocaciones al intérprete o instalaciones
52. de módulos o bibliotecas a través de pip, se va a hacer en el directorio que representa ese entorno virtual.
53. Que yo quiero salir del entorno virtual, quiero dejar de trabajar con él,
54. lo que hago es llamar a “deactivate”, y a partir de ese momento dejo de trabajar
55. con ese entorno virtual. Vemos la diferencia. Si yo digo que qué Python
56. se está ejecutando aquí, que no tengo ningún entorno virtual activo,
57. me dice que se está ejecutando el Python de usr/bin/python3, el Python 3 del sistema.
58. Si yo ahora activo el directorio del entorno virtual y hago lo mismo,
59. me dice que está ejecutando el Python 3 del entorno virtual,
60. y esto nos permite hacer cambios en las versiones de Python sin que haya modificaciones generales
61. en el sistema. Esto se mantendrá siempre. Desactivo y vuelvo a trabajar con el Python
62. 3 del sistema general. Entonces, ahora, por último, vamos a ver
63. cómo instalar un módulo en nuestro entorno virtual,
64. y para ello vamos a utilizar uno de los módulos que seguro que vamos a utilizar después para
65. el desarrollo web, porque es el que nos da toda la estructura
66. necesaria para las aplicaciones que vamos a desarrollar, que es el módulo Flask.
67. Si intentamos instalarlo, sin tener ningún entorno virtual activo, ¿qué va a ocurrir?
68. Que no me deja porque no tengo ningún directorio virtual activo.
69. Si activo el entorno virtual web, y lo repito, ahora sí que se conecta y sí que instala todo lo que necesita.
70. Pero veis dónde lo está instalando, lo está
71. instalando en el entorno virtual. Si ahora hago “ls .virtualenvs/web/lib”,
72. sigo teniendo Python3 pero, si veo los binarios, me ha metido Flask, que
73. es lo que yo necesitaba, que le he dicho que lo instale.
74. No lo ha instalado en el sistema, sino que ha bajado el módulo aquí.
75. [Fin de la transcripción. Saltar al inicio.](https://courses.edx.org/courses/course-v1:UAMx+WebApp+1T2019a/courseware/2062d8c9518447c7b1c6749f85df98df/1c322177492548f79c0c7f363b92bd81/1?activate_block_id=block-v1%3AUAMx%2BWebApp%2B1T2019a%2Btype%40vertical%2Bblock%402783ad7dc6f14b2fb032e39532163f17#transcript-start-82402fc855f54e8195e1f8d6fa0d1117)



Instrucciones que hemos utilizado en este vídeo (copia y pega en tu consola):

- Para comprobar si tenemos VirtualEnv instalado: `virtualenv`
- Para instalar VirtualEnv: `sudo apt install virtualenv`
- Para crear un directorio donde almacenar los entornos virtuales: `mkdir ~/.virtualenvs`
- Para crear el entorno virtual: `virtualenv ~/.virtualenvs/web`
- Impedir la instalación de módulos fuera de un entorno virtual: `export PIP_REQUIRE_VIRTUALENV=true`
- Permitir eliminar el valor de dicha variable de entorno: `unset PIP_REQUIRE_VIRTUALENV`
- Instalar módulo pprint: `pip3 install pprint`
- Para abrir fichero bashrc y especificar en él que debe haber un entorno activo para la instalación de módulos: `emacs .bashrc &`
- Activar entorno virtual: `source .virtualenvs/web/bin/activate`
- Desactivar el entorno virtual: `deactivate`
- Para conocer qué Python se está ejecutando: `which python3`
- Instalar módulo Flask (necesario tener el entorno virtual web activado): `pip3 install flask`