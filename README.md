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

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/11.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/12.PNG)

![Imagenes](https://github.com/danielrodriguezvillalba/ARSW-Laboratorio8/blob/master/images/13.PNG)

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
3. ¿Al cerrar la conexión ssh con la VM, por qué se cae la aplicación que ejecutamos con el comando npm FibonacciApp.js? ¿Por qué debemos crear un Inbound port rule antes de acceder al servicio?
4. Adjunte tabla de tiempos e interprete por qué la función tarda tando tiempo.
5. Adjunte imágen del consumo de CPU de la VM e interprete por qué la función consume esa cantidad de CPU.
6. Adjunte la imagen del resumen de la ejecución de Postman. Interprete:
* Tiempos de ejecución de cada petición.
* Si hubo fallos documentelos y explique.
7. ¿Cuál es la diferencia entre los tamaños B2ms y B1ls (no solo busque especificaciones de infraestructura)?
8. ¿Aumentar el tamaño de la VM es una buena solución en este escenario?, ¿Qué pasa con la FibonacciApp cuando cambiamos el tamaño de la VM?
9. ¿Qué pasa con la infraestructura cuando cambia el tamaño de la VM? ¿Qué efectos negativos implica?
10. ¿Hubo mejora en el consumo de CPU o en los tiempos de respuesta? Si/No ¿Por qué?
11. Aumente la cantidad de ejecuciones paralelas del comando de postman a 4. ¿El comportamiento del sistema es porcentualmente mejor?
