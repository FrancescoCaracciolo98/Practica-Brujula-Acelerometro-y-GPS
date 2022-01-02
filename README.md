# Practica Brújula, Acelerómetro y GPS
El objetivo de la práctica de esta semana consiste en utilizar los componentes más sencillos del 
móvil. Estos son: Brújula, Acelerómetro y GPS.


* **Asignatura:** Interfaces Inteligentes
* **Autor:** Francesco Caracciolo
* **Correo:** alu0101526621@ull.edu.es


## Parte Acelerómetro
Escribimos el script para poder aprovechar el acelerómetro que se encuentra dentro de un móvil. Dentro de mi teléfono hay un dispositivo que me dice la orientación de mi teléfono en el mundo real.


![Screenshot%20(5481)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5481).png)


Los ejes que Unity me da por defecto son los de la siguiente figura. 


![Screenshot%20(5475)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5475).png)


Pero quiero usar el teléfono de forma horizontal.
Para hacer esto, uso la línea de código

`tilt = Quaternion.Euler(90, 0, 0)*tilt;`


Entonces puedo crear un avión y colocar una esfera en él que luego puedo controlar gracias al acelerómetro.


![Screenshot%20(5476)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5476).png)


Para hacer la aplicación más interesante, creo un pequeño laberinto, como el de la imagen.


![Screenshot%20(5479)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5479).png)


![Screenshot%20(5484)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5484).png)


&nbsp;
 
## Parte GPS

GPS, global position system, es un sistema de navegación que muestra mi ubicación actual. Puedo obtener un conjunto de coordenadas, una ubicación de latitud norte y sur; y una ubicación de longitud este y oeste.


Veamos el código:


![Screenshot%20(5484)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5484).png)
![Screenshot%20(5483)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5483).png)


Usamos una corrutina porque tenemos que esperar a que el usuario responda, para dar permiso al dispositivo y a la aplicación remota Unity para usar la ubicación del GPS.

Grabo la latitud y la longitud.

&nbsp;
 
## Parte GPS
