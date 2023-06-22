
# Sistema de incendio con Arduino






## Demo

![](https://drive.google.com/file/d/1UtpIbJVPqqhiy1V4pZDgzANOKaG6MJUu/view?usp=drive_link)


## Integrante

* Carolina Gonzalez Parra
## Consigna

El objetivo de este proyecto es diseñar un sistema de incendio utilizando Arduino que pueda
detectar cambios de temperatura y activar un servo motor en caso de detectar un incendio.
Además, se mostrará la temperatura actual y la estación del año en un display LCD.

## Funcionalidad


* Se importaron las librerias necesarias para utilizar el Display LCD, ServoMotor y control IR
* Se definieron las variables necesarias para tomar valores, como la temperatura, saber el estado de la alarma, saber el estado actual y anterior de la estacion del año. 
* En el loop principal se hace uso de diferentes funciones:
     
     - leer_temperatura() hace una lectura del sensor de temperatura 
     - servo_giro() - activa el Servo
     - alarma_leds() - enciende y apaga los leds 
     - imprimir_mensaje/mensaje_alarma() - 2 funciones que imprimen un mensaje en eL Display LCD
     - leer_estacion() -evalua el rango de temperatura que se esta leyendo e imprime por el Display LCD los grados y la estacion del año dependiendo de la temperatura
     - activar_alarma() - activa el servo, enciende leds, imprime msj en el Display LCD
     - desactivar_alarma() - hace lo opuesto a activar_alarma()

 Presionando el boton de ON/OFF del control IR damos inicio al programa y se puede visualizar la temperatura actual junto con su estacion del año.
si la temperatura supera los 60 grados se activa la alarma de incendio que puede ser desactivada presionando el boton de FUNC/STOP del control. lo que daria por finalizado nuestro circuito.


## Link al Proyecto

[Link a Tinkercard](https://www.tinkercad.com/things/65HbKY1X9E9-gonzalez-carolina-2-parcial-spd/editel?sharecode=g2flcmuGaiL1eOBwNqKqYVtuZqweA9efQHscLeTH3Sc)
