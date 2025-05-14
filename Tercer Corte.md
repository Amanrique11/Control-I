# Indetificacion de sistemas  por curva de reaccion 
## 1. Indetificacion de sistemas en lazo abierto 
La identificacion de sistemas por curva de reacion es un tecnica utilizada en el campo de control de sistemas para obtener un modeol aproximado del comportamieno de un sistema a partir de su respuesta a una entrada escalon. Esta tecnica es muy util cuaudno no se tiene un modelo matematico exacto del sistema, pero si se puede medir como responde ante cirtos estimulos.
>🔑 *Curva de reaccion:* Es la respuesta temporal del sistema a un entrada escalon.
## 2. Procedimineto Basico 
1. Aplicar una entrada escalon al sistema.
2. Medir la salida del sistema con respecto al tiempo.
3. Obtener parametros clave de la curva:
  - Tiempo Muerto(L)
  - Constante de tiempo(T)
  - Ganancia del sistema(K)
>🔑 *Tiempo Muerto:* Tiempo entre la aplicacion del escalon y cuadno la salida comienza a cambiar.

>🔑 *Constante de tiempo:* Relacionado con la rapidez con que la salida alncanza  su valor final.

>🔑 *Ganancia del sistema:* Cambio en la salida divido entre el cambio en la entrada.

## 3. Modelo tipico: Sistema de primer orden con retardo
$$G(s) = \frac{K*e^{-Ls}}{Ts+1}$$

Donde:
- K: Ganancai estatica.
- T: Costante de tiempo.
- L: Tiempo muerto.

## 4. Otros metodos de optener un modelo de planta
- Modelo matematico (Ecuaciones diferenciales).
- Identificacon de parametros en lazo cerrado.
- Analisis en frecuencia.
- Tecnica de inteligencia computacional.

## 5. Metodo empirico 
Se basa en obtener un modelo matematico aproximado de un proceso a partir de datos experimentales, sin necesidad de conocer su estructura interna. Este enfoque es especialemnte util en sistemas industriales donde la dinamica completa es compleja o desconociada.

