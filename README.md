# TECTIJUANA
## SERVO Y ROTARY DIALER
### POR: JAVIER SANCHEZ

![](https://i.imgur.com/ttzBwm6.png)

## ¿Que es?

El servomotor es un dispositivo eléctrico que se puede utilizar para girar objetos (como el brazo robótico) con precisión.
El servomotor consiste en un motor de CC con mecanismo de retroalimentación negativa de detección de errores. Esto permite un control preciso sobre la velocidad angular y la posición del motor. En algunos casos, se utilizan motores de CA.
Es un sistema de circuito cerrado donde utiliza retroalimentación negativa para controlar el movimiento y la posición final del eje.
No se utiliza para la rotación continua como los motores convencionales de CA / CC.
Tiene un ángulo de rotación que varía de 0° a 180°.

## Mecanismo

Como se muestra en la figura anterior, el servomotor tiene tres pines para su funcionamiento como,

#### +VCC (ROJO)
- Conecte la fuente +VCC a este pin. Para SG90 Micro Servo es de 4.8 V (~5V).

#### Suelo (MARRÓN)
- Conecte Ground a este pin.

#### Señal de control (NARANJA)
- Conecte PWM de 20 ms (50 Hz) a este pin.

## Caracteristicas de un servo modelo Micro Servo Tower-pro

| Velocidad        | 0.10 sec/60° @ 4.8V |   |   |   |
|------------------|---------------------|---|---|---|
| Torque           | 1.8 Kg-cm @ 4.8V    |   |   |   |
| Voltaje          | 3.0-7.2V            |   |   |   |
| Temp. De Funcion | -30 ℃ ~ 60 ℃        |   |   |   |

![](https://www.electronicwings.com/storage/PlatformSection/TopicContent/134/description/Servo_Motor_Mechanism.png)

## Principal Funcionamiento

#### Consiste en motor de CC, conjunto de engranajes y circuitos de control de retroalimentación. La señal PWM se utiliza para controlar el servomotor. Se aplica en el pin de la señal de control.
#### Los circuitos de control de retroalimentación servo contienen un comparador que compara la señal de control (PWM) y la señal de referencia del potenciómetro para generar una señal de error que luego se amplifica y se le da al motor de CC.
#### El eje del motor de CC está conectado al eje del potenciómetro (perilla) a través del conjunto de engranajes. Por lo tanto, el motor de CC giratorio gira el potenciómetro, que en términos cambia la señal de referencia del potenciómetro dada al comparador.
#### En alguna posición del eje, tanto la señal del potenciómetro como la intensidad de la señal de control coinciden, lo que produce una salida de señal de error cero. Por lo tanto, la rotación continúa hasta que la señal de error de salida del comparador se vuelve cero y el motor de CC se detiene.

## Codigo de funcionamiento servo el CircuitPython con Pico w.

![](https://i.imgur.com/KyCEmuo.png)

## Imagen GIF demostracion de la practica.
![](https://i.imgur.com/lJyaw9k.gif)


#
#

![](https://i.imgur.com/YtN6IQj.png)

## ¿Que es?

Es un componente de un teléfono que implementa una tecnología de señalización en telecomunicaciones conocida como marcación por pulsos. Se utiliza al iniciar una llamada telefónica para transmitir el número de teléfono de destino a una central telefónica. En el dial giratorio del teléfono, los dígitos están dispuestos en un diseño circular para que una rueda de dedo se pueda girar contra la tensión del resorte con un dedo. Comenzando desde la posición de cada dígito y girando hasta la posición fija de parada del dedo, el ángulo a través del cual se gira el dial corresponde al dígito deseado. Los teléfonos compactos con el dial en el teléfono tenían todos los orificios igualmente espaciados en el dial, y un tope de dedo con resorte con un recorrido limitado.

## Funcion

Para marcar un número, el usuario coloca un dedo en el orificio del dedo correspondiente y gira el dial en el sentido de las agujas del reloj hasta que llega a la parada del dedo. Luego, el usuario saca el dedo y un resorte en el dial lo devuelve a la posición de reposo. Por ejemplo, si el usuario marca "6" en un teléfono norteamericano, los contactos eléctricos operados por una leva en el eje del dial y una pata se abrirán y cerrarán seis veces a medida que el dial regrese a la posición de inicio, enviando así seis pulsos a la oficina central. Los diales británicos y australianos funcionan de la misma manera.

Se utilizan diferentes sistemas de pulsos, que varían de un país a otro. Por ejemplo, Suecia utiliza dos pulsos para señalar el número cero y 11 pulsos para señalar el número nueve. Nueva Zelanda utiliza diez pulsos menos el número deseado; por lo que marcar 7 produce tres pulsos. En Noruega, se utilizó el sistema norteamericano con el número '1' correspondiente a un pulso, a

## Muelle de Retroceso

Los primeros diales funcionaban por acción directa o directa. Los pulsos se generaron a medida que el dial giraba hacia la posición de parada del dedo. Cuando el movimiento de la mano del usuario era errático, producía los números equivocados. A finales del siglo 19, la esfera se refinó para funcionar automáticamente por un resorte de retroceso. El usuario seleccionó el dígito que se iba a marcar, giró el dial hasta el punto del dedo y, a continuación, lo soltó. El resorte hizo que el dial volviera a girar a su posición de inicio, durante el cual se mantuvo una velocidad constante con un regulador centrífugo.

## Ejemplo Fisico

![](https://i.imgur.com/PhqVUnY.png)
