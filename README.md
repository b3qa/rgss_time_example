﻿# EJEMPLO DE EVENTO PARA RPG MAKER XP

 ### Introducción

 El siguiente es un ejemplo básico de como construir un evento que se activa dependiendo del día de la semana (fecha de sistema).

 ### Requisitos
 * **RPG Maker XP** [Steam](https://store.steampowered.com/app/235900/RPG_Maker_XP/) [Web oficial](https://www.rpgmakerweb.com/products/rpg-maker-xp) 

### Instalación
* Clonar o descargar el repositorio (descomprimir si es necesario)
* Abrir RPG Maker XP
* En *Archivo &rarr; Abrir Proyecto* seleccionar la carpeta del proyecto
* Seleccionar *Game.rxproj*

### Funcionamiento

El codigo principal que asigna un valor a una variable del RPG Maker es el siguiente:

```ruby
t = Time.now
$game_variables[2] = t.wday
```

Donde
* **Time.now** obtiene la fecha del sistema
* **$game_variables** es el objeto que contiene las variables de RPG Maker, se puede cambiar elegir cualquier variable del array para almacenar el dato
* **t.wday** es el día de la semana empezando por *0 = Domingo* hasta *6 = Sábado*

Una vez asignada la variable se procede a hacer una comparación usando el sistema de eventos de RPG Maker.

### Guía del juego

El objetivo del juego es entrar a la Mazmorra Semanal, para lograr entrar se debe visitar el día correspondiente (En el cartel a la derecha de la entrada se puede ver el día de la semana que abre la mazmorra)

Personajes:
* **Heroe:** Eres tu, un aventurero que ha venido a probar su suerte en la mazmorra.
* **Aventurera pelirroja:** Otra aventurera que también esta a la espera de que se abra la puerta.
* **Guardia de la mazmorra:** Su misión es abrir la puerta a los aventureros cuando llegue el día indicado.
* **???:** ¿De quien se trata? Quien sabe, pero al parecer planea hacer trampa.
