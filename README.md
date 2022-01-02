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


![Screenshot%20(1)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(1).png)
![Screenshot%20(5483)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5483).png)


Usamos una corrutina porque tenemos que esperar a que el usuario responda, para dar permiso al dispositivo y a la aplicación remota Unity para usar la ubicación del GPS.

Grabo la latitud y la longitud.


![Screenshot%20(2)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(2).png)

&nbsp;
 
## Parte Brújula

Finalmente, como última parte, usemos la función de brújula de mi teléfono.

Para hacer esto, el código es el siguiente:


![Screenshot%20(5487)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5487).png)


Para capturar la orientación norte, utilizo un rectángulo rojo.


![Screenshot%20(5488)](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/Screenshot%20(5488).png)

&nbsp;
 
## Conclusión del trabajo

Ahora veamos cómo funcionan estas tres partes en la misma aplicación:


![V2.0_Practica%20Br%C3%BAjula%2C%20Aceler%C3%B3metro%20y%20GPS%20-%20SampleScene%20-%20Android%20-%20Unity%202020.3.20f1%20_DX11_%202022-01-02%2018-39-12.gif](https://github.com/FrancescoCaracciolo98/Practica-Brujula-Acelerometro-y-GPS/blob/main/V2.0_Practica%20Br%C3%BAjula%2C%20Aceler%C3%B3metro%20y%20GPS%20-%20SampleScene%20-%20Android%20-%20Unity%202020.3.20f1%20_DX11_%202022-01-02%2018-39-12.gif)
