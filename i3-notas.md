# i3 Window Manager

## Info/Reference

### Cómo gestionar ventanas (WIP)

#### Abrir aplicaciones

- Abrir terminal $mod+Enter
- Menú $mod+d (requiere conocer el nombre de la aplicación tal y como se lanza desde línea de comando)

#### Ventanas

- Cambiar el foco de ventana: $mod+<cursor>
- Mover la ventana $mod+Shift+<cursor>

- Poner la ventana a pantalla completa $mod+f / Salir de pantalla completa $mod+f

- Dividir ventana verticalmente (antes de abrir nueva ventana) $mod+v (en horizontal $mod+h)
- cambiar tamaño de una ventana $mod+r (seguido de los cursores)
- Cerrar una ventana: $mod+Shift+q

- Convertir una ventana en "flotante": $mod+Shift+<espacio> (al repetir la combinación se vuelve a la cuadrícula)

- Cambiar el modo en el que se muestran las ventanas:
  - Como pestañas: $mod+w
  - En vertical u horizontal $mod+e (por defecto las ventanas se muestran una junto a otra, de lado, mientras que con $mod+e pasarían a estar una sobre otra, en vertical) También aplica a las nuevas ventanas que se abran.
  - Apiladas: $mod+s

#### Workspaces

- Cambiar de Workspace: $mod+<número de workspace>

#### Cambios en i3

- Reiniciar i3: $mod+Shift+r
- Recargar la configuración de i3: $mod+Shift+c
- Salir de i3: $mod+Shift+e

### Editar el fichero de configuración  
  
El fichero de configuración de i3 se encuentra en ~/.config/i3/config

#### Aplicaciones

En la configuración de i3wm, `bindsym` crea un nuevo atajo; `exec` lanza un programa.

Por ejemplo, para lanzar Firefox:

```config
bindsym $modhift+b exec firefox
```

#### Barra de estado

La configuración de la barra de estado se encuentra en la sección `bar`. En `status_command` se indica qué barra se usa; por defecto, se usa `i3status` pero existen otras barras como `i3blocks`, `lemonbar` o `polybar`.

En esta sección también se puede cambiar la posición de la barra.


## Open Issues

### La letra es muy pequeña en todas las aplicaciones por defecto (en una pantalla 4K)

Al parecer hay algunos resultados al buscar en Google. Tengo que mirarlo con más detalle.

> Temporalmente he aumentado el tamaño de la fuente en el editor del sistema.

En la configuración de i3, el tamaño y fuente de los títulos de las ventanas se puede configurar mediante:

```config
font pango:monospace 14
```
   
Application launcher -> rofi
Flameshoot -> screenshot
dunst -> notificaciones
