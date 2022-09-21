# TECTIJUANA
## SENSOR SERVO
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

![](https://www.electronicwings.com/storage/PlatformSection/TopicContent/134/description/Servo_Motor_Mechanism.png)

## Principal Funcionamiento

#### Consiste en motor de CC, conjunto de engranajes y circuitos de control de retroalimentación. La señal PWM se utiliza para controlar el servomotor. Se aplica en el pin de la señal de control.
#### Los circuitos de control de retroalimentación servo contienen un comparador que compara la señal de control (PWM) y la señal de referencia del potenciómetro para generar una señal de error que luego se amplifica y se le da al motor de CC.
#### El eje del motor de CC está conectado al eje del potenciómetro (perilla) a través del conjunto de engranajes. Por lo tanto, el motor de CC giratorio gira el potenciómetro, que en términos cambia la señal de referencia del potenciómetro dada al comparador.
#### En alguna posición del eje, tanto la señal del potenciómetro como la intensidad de la señal de control coinciden, lo que produce una salida de señal de error cero. Por lo tanto, la rotación continúa hasta que la señal de error de salida del comparador se vuelve cero y el motor de CC se detiene.
