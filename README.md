# Laser DogFight

# VERSION ACTUAL v0.2a

## Caracteristicas:
* Funciona Conectado a un canal cualquiera, sin necesidad de alimentación adiccional 
* Bajo consumo teórico. (pico teórico de corriente máxima, 200mA.  Consumo medio <10 mA)
* Se utilizan fototransistores IR de 38khz, eliminando la necesidad de filtros de banda y amplificadores.
* Sistema de daños "realistas", se necesita más de 1 impacto para derribar, no siempre se derriba en el mismo nº de impactos.
* Se incluye la posibilidad de añadir buzzer y LEDS para flashes de aviso de daño y derribo
* Construcción modular, modulos basicos: CPU, laser y receptor. Extra: LEDS externos


## Funcionamiento:
 El sistema básico consta de un emisor IR y un receptor IR.
 En la version actual, el receptor se posiciona en la cola del aparato, y el emisor en cualquier parte de la aeronave, siempre que   apunte hacia adelante y esté alineado con el plano horizontal de vuelto.

 Conectar el modulo CPU al receptor, en el canal que se desee tener el "disparo".
 
 
 #### Antes de volar con el dispositivo, es recomendable colimar el haz IR. Para ello, el modulo debe estar conectado a cualquier canal y el receptor encendido. Pulsaremos el boton "test", lo cual encenderá el haz de luz visible. Debemos estar en una habitación un poco oscura, para poder ver la proyeccion del LED.#### 
 
 Alejando o acercando el tubo colimador, debemos hacer que el haz sea lo más pequeño posible. Recomendable hacerlo a una distancia de +5m.  Debido a la posición del led de pruebas, el haz nunca va a estar alineado con el eje horizontal/vertical del avión, esto es normal y no significa que el haz IR esté desalineado.
 
 ###  EN VUELO
  Actualmente el sistema tiene munición ilimitada y sistema de simulación de daños aleatorios.
  
  El atacante debe posicionarse en la cola del enemigo y apuntando con su morro hacia el objetivo. Al presionar el botón asignado a disparo, se disparará una ráfaga IR ilimitada hasta que se deje de disparar.  Si el objetivo es alcanzado, éste emitira una señal auditiva y luminosa.
  
  Se deberá alcanzar varias veces a un objetivo para derribarlo (el daño por impacto es aleatorio)
  
  Si eres derribado, el disparo queda anulado y deberás aterrizar, para resetear el sistema.
  
  #### Significado de avisos
  * Luz verde, 2 flash cada 1s:  Status ok. Sin daños.
  * Luz verde, 1 flash cada 1s:  Daños leves. Daños < 50%.
  * Luz roja , 1 flash cada 1s:  Daños graves. Daños >50%.
  * Flashes rojos y pitidos rápidos: Derribado.  Despues de 4seg dejará de pitar y sólo parpadeara el rojo cada 1/2s
  * Pitido corto + 1 flash rojo: impacto


# TODO
* Script para OpenTX
* Posibilidad de datos de telemetría
* Versión drones
