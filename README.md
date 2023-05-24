# Realizado por:
- García Angeles Belen 

# Proyecto: 
- Montacargas para un hospital

![Tinkercad](./imagenes/circuito.png)

# Descripción:
Se desarrollo un sistema a travez del cual podemos subir, bajar o pausar el montacargas de un hospital.

# Elemtos utilizados:
- Un arduino Uno
- Display de 7 segmentos
- Un led Rojo
- Un led Verde
- Tres botones

# Funcinamiento general:
Mediante la utilizacion de un arduino Uno, se programo un display de 7 segmentos el cual nos indica el piso 
en el que se encuentra nuestro montacargas. Para poder subir, bajar o pausar nuestro montacargas utilizaremos los botones.
- En caso de seleccionar subir o bajar nuestro montacragas realizara dicha accion y en conjunto encendera un led verde que 
nos indicara que el montacargas se encuentra en movimiento. A su vez el numero de piso se vera reflejado en el display de 7 
segmentos. 
- Si por otra parte, seleccionamos pausa el montacarga se detendra y se encendera un led rojo que indicara que el montacarga
se detuvo, el mismo no volvera a moverse a no ser que el boton subir o bajar se presione. 

# Codigo - Funciones Principales:

- void leer_estado_boton(int boton) --> Esta funcion lee el estado de cualquier boton que reciba por parametro.

- subir_montacarga(int contador) --> Esta funcion recibe un contador y realiza la tarea de modificar el display de 7 segmentos para indicar que el montacarga sube. Tambien llama a funcion para encender el led verde y nos retornara en que piso quedo nuestro display.

- bajar_montacarga(int contador) --> Esta funcion recibe un contador y realiza la tarea de modificar el display de 7 segmentos para indicar que el montacarga baja. Tambien llama a funcion para encender el led verde y nos retornara en que piso quedo nuestro display.

- pausar_montacarga() --> Esta funcion pausa el montacargas, detiene el funcionamiento hasta que se presione subir o bajar. Nos retornara 1 o 0 que nos indicara si el sistema esta pausado o no. 

- control_montacarga(int contador) --> Esta funcion controla al montacargas, leyendo los estados de los botones que se presionan y actuando en consecuencia. ESta funcion recibira un contador y nos retornara ese mismo contador modificado.

- numeros(int contador) --> Esta funcion nos permite mostrar en el display de 7 segmentos el numero que se pase en el parametro contador. 


# Link al proyecto:
- Tinkercad: https://www.tinkercad.com/things/hnSr59MyaD9-parcial-spd-garcia-angeles-belen-1b/editel?sharecode=VRNFzka11C9dcUpGZAGHC3VY3ogpH4FpOKJKRxT265M
- Codigo GDB: https://onlinegdb.com/kDX3u2RYl
