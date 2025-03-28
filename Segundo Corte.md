# Sistemas de Segundo Orden
## ¿Que es?
Un sistema de seguhndo orden es aquqel funcion de tranferencia tiene dos polos. Al igual que en los sistemas de primer orden, en cual quier fisico real el numero de ceros debe ser inferior o igual al de los polos, y por ello los sistemas de segundo orden pueden tener maximo dos ceros
## Ecuacion General
$$G(S) = \frac{c}{s^2 +  a \cdot s + b}$$




## Ecuacion canonica

$$G(s) = \frac{K \cdot \omega_n^2}{s^2 + 2\zeta\omega_n s + \omega_n^2}$$

Donde:
K = Ganancia estatica.

$\zeta$ = Factor de amotiguamineto .

$\omega_n$ = Frecuencia Natural

## ¿Dinamica de los sistemas de Segundo Orden

El comportamiento dinamico de un sistema de segundo oirden puede ser descrito en terminos de dos parametros $\zeta$ y $\omega_n$.
Dependiendo del valor que tome $\zeta$ el sistema tendra diversos comportamientos, los cuales son:

$\zeta = 0$ - Sistema Oscilatorio

$0 < \zeta < 1$  - Sistema Subamortiguado

$\zeta = 0$ - Sistema Criticamente amoritguado

$\zeta > 1$ - Sistema Sobre  Amortiguado 
 ### Variacion del factor de amortiguamiento 

 ![image](https://github.com/user-attachments/assets/5da71048-4278-4401-a104-7c09be6a83a7)

### Variacion de la frecuencia Natural No Amortiguada

![image](https://github.com/user-attachments/assets/cb691ee6-80ae-4514-9e79-1ae6b0903a4a)

## Polos de los sistemas de sistemas
Partiendo de la ecuacion canonica de un sistema de segundo orden, los polos estan dado caudno el denomindaro se iguala a cero.

$$s^2 + 2\zeta\omega_n s + \omega_n^2 = 0$$

Aplicamos la ecuacion general para encontrar las reices del polimonio.

$$s_{1,2} = \frac{-2\zeta\omega_n \pm \sqrt{4\zeta^2\omega_n^2 - 4\omega_n^2}}{2}$$

$$s_{1,2} = \frac{-2\zeta\omega_n \pm \sqrt{4\omega_n^2(\zeta^2 - 1)}}{2}$$

Los polos del sistemas de segundo orden son:

$$s_{1,2} = -\zeta\omega_n \pm \omega_n \sqrt{\zeta^2 - 1}$$

## Sistema Oscilatorio

Es un sistema que posee sus polos unicamente con componentes imaginarias

![image](https://github.com/user-attachments/assets/28910c30-83ad-4bd6-bc5f-6a672b3e81d4)

### Respuesta transitoria del sistema oscilatorio

![image](https://github.com/user-attachments/assets/275a30c0-6f93-4d2a-9873-4a39afd5d4de)

