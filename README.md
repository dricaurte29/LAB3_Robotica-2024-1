# Laboratorio 3 de Robótica: Desarrollo e Introducción a ROS

- David Andrés Ricaurte de Lima  
  Ingeniería Mecatrónica  
  Universidad Nacional de Colombia  
  Bogotá, Colombia  
  dricaurte@unal.edu.co

- Juan Antonio Rojas Cobos  
  Ingeniería Mecatrónica  
  Universidad Nacional de Colombia  
  Bogotá, Colombia  
  juarojascog@unal.edu.co

Este laboratorio tiene como principal objetivo de adquirir conocimientos y habilidades referentes a los conceptos básicos de ROS(Robot Operating System), a los comandos fundamentales de ROS, a la conexión de nodos de ROS y Matlab y a la conexión inicial de motores Dynamixel con ROS. Brindando así una introducción practica a ROS,a la interacción de este con Matlab y a la conexión de motores Dynamixel proporcionando una base sólida para trabajar en proyectos de robótica y de desarrollo de sistemas robóticos.

## Descripción de la Solución Planteada Matlab

Primer Script: https://github.com/dricaurte29/LAB3_Robotica-2024-1/blob/5e2bddc1a95a71f3d0e96a30c07e136c9d061fca/scriptsMatlab/turtle.m

En este código, se inicializa ROS, crea un publicador para enviar comandos de velocidad para el control de la tortuga, establece una velocidad lineal en 2, envia el comando de velocidad y luego realiza una pausa durante 1 segundo.

![Funcionamiento del primer script](media/rosmat1.png)

Segundo Script: https://github.com/dricaurte29/LAB3_Robotica-2024-1/blob/5e2bddc1a95a71f3d0e96a30c07e136c9d061fca/scriptsMatlab/turtle1.m

En este código se realiza una conexión con el nodo de ROS, se obtiene información referente a la posición y orientación de la tortuga y luego cierra la conexión con ROS.

![Funcionamiento del segundo script](media/robmat2.png)

Tercer Script: https://github.com/dricaurte29/LAB3_Robotica-2024-1/blob/5e2bddc1a95a71f3d0e96a30c07e136c9d061fca/scriptsMatlab/turtle2.m

En este código se establece una conexión con ROS, se utiliza un servicio para teleportar la tortuga a una nueva posición y orientación, y luego se cierra la conexión con ROS.

![Funcionamiento del tercer script](media/rosmat3.png)

## Descripción de la Solución Planteada Python
Script: https://github.com/dricaurte29/LAB3_Robotica-2024-1/blob/5e2bddc1a95a71f3d0e96a30c07e136c9d061fca/scriptsPython/myTeleopKey.py

Este script Python proporciona un controlador para una tortuga simulada en el paquete Turtlesim de ROS (Robot Operating System). Permite controlar los movimientos y la orientación de la tortuga utilizando las teclas del teclado.

### Funcionamiento

El script incluye las siguientes funciones principales:

- `move_forward()`: Mueve la tortuga hacia adelante.
- `move_backward()`: Mueve la tortuga hacia atrás.
- `rotate_clockwise()`: Gira la tortuga en sentido horario.
- `rotate_counterclockwise()`: Gira la tortuga en sentido antihorario.
- `reset_pose()`: Teletransporta la tortuga a la posición y orientación centrales.
- `rotate_180_degrees()`: Teletransporta la tortuga para girar 180 grados.

Además, el script utiliza la función `getkey()` para obtener la entrada del teclado sin necesidad de presionar Enter, y un bucle principal para detectar las teclas presionadas y llamar a las funciones correspondientes del controlador.

Este código se encarga de controlar un robot tortuga en el entorno ROS desde python mediante entradas de teclado:
- W: Movimiento hacia adelante
- S: Movimiento hacia atrás
- A: Rotación antihoraria
- D: Rotación horaria
- R: Regrasar a posición y orientación central
- SPACE: Girar 180

En el siguiente video se aprecia el funcionamiento de este código:
https://youtu.be/DN9ZJ2M9to4
