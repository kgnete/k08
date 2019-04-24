[README](README.md)

## Instalación Python 3

 Marcar esta página

La tecnología que vamos a utilizar para desarrollar funcionalidad del lado del servidor va a ser Python. Concretamente, vamos a utilizar Python 3 porque, aunque Python 2 sigue vivo, ya tiene fecha de caducidad (2020).

Si tienes en tu máquina una versión de Linux relativamente reciente, es muy probable que tengas varias versiones de Python instaladas: tanto Python 2 como Python 3, y entonces este paso de instalación te lo puedas saltar.

Los pasos que vamos a seguir están tomados de una de las web fundamentales con instrucciones para la utilización de Python: [The Hitchhiker’s Guide to Python](https://docs.python-guide.org/starting/install3/linux/).

### 















0:00 / 0:00

Velocidad: Presiona ARRIBA para acceder al menú, luego usa las teclas de ARRIBA y ABAJO para cambiar a diferentes velocidades, y presiona ENTER para cambiar a la velocidad seleccionada.

Haz clic en este botón para silenciar o activar el sonido del vídeo o usa los botones ARRIBA o ABAJO para aumentar o disminuir el nivel de volumen.

Máximo Volumen.



### Transcripción de video

1. [Inicio de la transcripción. Saltar al final.](https://courses.edx.org/courses/course-v1:UAMx+WebApp+1T2019a/courseware/2062d8c9518447c7b1c6749f85df98df/1c322177492548f79c0c7f363b92bd81/1?activate_block_id=block-v1%3AUAMx%2BWebApp%2B1T2019a%2Btype%40vertical%2Bblock%402783ad7dc6f14b2fb032e39532163f17#transcript-end-770cf066b9334e659a3caca8900f8258)
2. Bien, pues vamos a empezar con la instalación.
3. Como decía antes, el primer paso es instalar Python 3 o, en su defecto, verificar que ya lo tenemos instalado.
4. Entonces, para ello nos abrimos un terminal.
5. Tecleamos aquí “python” y está instalado, cuando yo lo ejecute me va a abrir el intérprete de Python.
6. Y concretamente, me ha abierto el intérprete de Python 2.7.15.
7. Me está abriendo una versión de Python 2 que no nos interesa para el curso, necesitaría
8. una versión de Python 3.
9. Como os comentaba antes, las distribuciones actuales de Ubuntu y en general de casi cualquier
10. Linux vienen con versiones de Python 2 y Python 3 por defecto.
11. Entonces, ¿cómo vemos qué versiones tenemos instaladas?
12. Hay otros mecanismos, pero uno rápido es teclear “python”,
13. dar al tabulador para ver qué opciones me ofrece y aquí vemos,
14. que tengo esos 5 comandos para ejecutar Python.
15. Estas son las versiones de Python 2 que tengo instalada en mi máquina
16. y la versión de Python 3 que tengo instalada en mi máquina.
17. Entonces, esta distribución de Ubuntu, ya por defecto, trae una versión de Python 2 y de Python 3.
18. La de Python 2 en concreto es la 2.7.15 que veíamos,
19. y para ver la de Python 3 simplemente tenemos que ejecutar este comando (“python3.6”),
20. y vemos que es la 3.6.5 de Python 3. Python 3 está enlazado a Python 3.6.
21. Si ejecuto “python3” me abre el intérprete de Python 3.6.5.
22. Si ejecuto Python 2, me abre el intérprete de Python 2.7.15
23. y si ejecuto Python, me vuelve a abrir también el intérprete de Python 2.7.15.
24. En nuestro caso, ya tendríamos instalado Python 3 en su versión más reciente, que
25. es lo que necesitamos en el curso.
26. Si no estuviera instalado, si una vez que hacemos esto vemos que no tenemos Python 3,
27. lo que tenemos que hacer es utilizar el gestor de paquetes de vuestra distribución (en el caso de Ubuntu,
28. el gestor de paquete es apt), y decirle que queremos instalar Python 3: “apt sudo install python3”.
29. Entonces, si yo ejecuto esto y no tengo nada instalado, me descargaría los paquetes;
30. al ya tenerlo instalado, ¿qué es lo que me dice? Que Python 3 ya está en su versión más reciente.
31. Para ver cómo funcionaría el apt para instalar el paquete de Python, vamos a instalar pip,
32. que es el gestor de paquetes de Python, para instalar módulos de Python que necesitemos,
33. y que ese sí que no viene instalado por defecto en prácticamente ninguna distribución de Linux,
34. y en esta en concreto no está instalado.
35. Entonces, si yo escribo “pip3”, que sería el gestor de paquetes para Python 3,
36. no existe ese comando, no existe esa utilidad en mi distribución, y me sugiere cómo instalarlo.
37. Y, exactamente igual que antes “sudo apt install de python3-pip”.
38. Entonces, vamos a ver qué es lo que hace apt a la hora de instalarlo.
39. Ejecuto esto, me dice todo lo que se tiene que bajar, todo lo que tiene que instalar.
40. Le digo que sí (S) para instalar, y después de esperar el tiempo necesario
41. para que se descargue todo lo que necesita y todas sus dependencias, después de terminar,
42. ya tendré disponible pip3 en mi máquina.
43. [Fin de la transcripción. Saltar al inicio.](https://courses.edx.org/courses/course-v1:UAMx+WebApp+1T2019a/courseware/2062d8c9518447c7b1c6749f85df98df/1c322177492548f79c0c7f363b92bd81/1?activate_block_id=block-v1%3AUAMx%2BWebApp%2B1T2019a%2Btype%40vertical%2Bblock%402783ad7dc6f14b2fb032e39532163f17#transcript-start-770cf066b9334e659a3caca8900f8258)



Instrucciones que hemos utilizado en este vídeo (copia y pega en tu consola):

- Ver qué versiones de Python tenemos instaladas: `python + tabulador`, para ver con qué autocompleta.``
- Instalar Python: `sudo apt install python3`
- Instalar el gestor de paquetes de Python, pip: `sudo apt install python3-pip`