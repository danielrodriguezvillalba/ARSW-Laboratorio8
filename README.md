### Escuela Colombiana de Ingeniería Julio Garavito 
### Arquitecturas de Software - ARSW

### Integrantes

* Daniel Felipe Rodriguez Villalba

### Parte 0 - Entendiendo el escenario de calidad

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/1.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/2.PNG)

### Parte 1 - Escalabilidad vertical

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/3.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/4.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/5.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/6.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/7.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/8.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/9.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/10.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/11.png)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/12.png)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/13.png)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/CPU.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/14.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/15.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/16.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/CPU2.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/17.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/18.PNG)



Preguntas

1. ¿Cuántos y cuáles recursos crea Azure junto con la VM?

`Para cada maquina virtual que se instancia en azure se crean 6 recursos`
* `Direccion IP publica`
* `Grupo de seguridad de red`
* `Interfaz de red`
* `Disco`
* `Red virtual`
* `Cuenta de almacenamiento`

2. ¿Brevemente describa para qué sirve cada recurso?

* `Direccion IP publica: Es el recurso que se encarga de la direccion IP para poder asi establecer comunicacion con otros recursos u otras maquinas.`
* `Grupo de seguridad de red: Es el recurso encargado del manejo del trafico hacia la maquina, en otras palabras filtra los datos que pasan y los que no hacia esta.`
* `Interfaz de red: Es el recurso encargado de la comunicacion entre la maquina y sus recursos locales, ademas de su comunicacion hacia internet.`
* `Disco: Es el recurso encargado de el almacenamiento local de la maquina.`
* `Red virtual: Es el recurso encargado de establecer una comunicacion segura entre maquinas de azure por medio de internet`
* `Cuenta de almacenamiento: Recurso encargado de el almacenamiento local de la maquina `

3. ¿Al cerrar la conexión ssh con la VM, por qué se cae la aplicación que ejecutamos con el comando npm FibonacciApp.js? ¿Por qué debemos crear un Inbound port rule antes de acceder al servicio?

`
Al cerrar la conexion SSH se cae la aplicacion porque la aplicacion esta corriendo para todo el publico mientras la conexion esta abierta con esta, sin embargo cuando la cerramos es por esto que se cae la conexion

Es necesario crear un Inbound Port Rule para permitir el acceso a esta aplicacion sea publico y se pueda consultar y usar desde internet
`

4. Adjunte tabla de tiempos e interprete por qué la función tarda tando tiempo.

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/14.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/17.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/15.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/18.PNG)

` Al pedir el calculo de todos estos numeros de fibonacci y hacerlo con una sola instancia de la maquina se torna muy lento el resultado por lo cual es necesario cambiar el almacenamiento de esta maquina pata que este escale verticalmente.` 

5. Adjunte imágen del consumo de CPU de la VM e interprete por qué la función consume esa cantidad de CPU.

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/CPU.PNG)

` Al pedir el calculo de todos estos numeros de fibonacci y hacerlo con una sola instancia de la maquina se torna muy lento el resultado por lo cual es necesario cambiar el almacenamiento de esta maquina pata que este escale verticalmente.
`

6. Adjunte la imagen del resumen de la ejecución de Postman. Interprete:
* Tiempos de ejecución de cada petición.
* Si hubo fallos documentelos y explique.

`B1ls :`

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/14.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/17.PNG)

`B2ms :`

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/15.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/18.PNG)



7. ¿Cuál es la diferencia entre los tamaños B2ms y B1ls (no solo busque especificaciones de infraestructura)?

`La principal diferencia yace en la escalablidad que cada una presenta frente a grandes cantidades de datos, afectando esto el desempeño de la aplicacion.
`

8. ¿Aumentar el tamaño de la VM es una buena solución en este escenario?, ¿Qué pasa con la FibonacciApp cuando cambiamos el tamaño de la VM?

`Cuando cambiamos el tamaño de la VM se aumenta la disponibilidad en mayor cantidad de datos, la solucion no es muy buena ya que nos genera un costo demasiado alto como para la funcionalidadque presta la aplicacion.`

9. ¿Qué pasa con la infraestructura cuando cambia el tamaño de la VM? ¿Qué efectos negativos implica?

`Como se ha venido mencionando en los puntos anteriores los efectos negativos son principalmente los costos que generan este tipo de almacenamientos, ademas que la busqueda de numeros tan grandes no se va a realizar con mayor frecuencia.`

10. ¿Hubo mejora en el consumo de CPU o en los tiempos de respuesta? Si/No ¿Por qué?

`Si, ya que al mejorar el rendimiento de la CPU se mejoran los tiempos de respuesta, esto debido al nuevo almacenamiento `

