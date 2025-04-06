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

## Sistema Subamortiguado

Es aquel que poseee  un par de polos complejos conjigados dentro de un sistema de segundo orden.

![image](https://github.com/user-attachments/assets/da18b3c7-62bc-4551-97d5-c6758ae23831)
### Respueta de uns sistema Subamortiguado

![image](https://github.com/user-attachments/assets/025dab07-1d57-4694-85e8-21f770051616)

Donde: 

Tp = Tiempo pico

Mp = Maximo Sobreimpulso

Td = Tiempo de desplazmamiento 

Ts = Tasa de Establecimineto 


### Analisis ananilitico de un sistema subamortiguado
En un sistema Subeamortiguado podemos hallar diferentes valores que nos ayuden a controlar la respuesta de la funcion de transferencia.

Donde podemos controlar en que momento queremos que tiempo queremos este la priemra subida en la respuesta:

$$t_p = \frac{\pi}{\omega_n \sqrt{1 - \zeta^2}}$$

Tambien podemos saber cual es el sobre impulso que hay entre el valor mas alto y el valor cuando el sistema ya esta estable. 

$$MP = \frac{y(t_p) - y(\infty)}{y(\infty) - y(0)} = e^{\frac{-\zeta\pi}{\sqrt{1 - \zeta^2}}}$$

Tambien podemos analizar en que tienpo el sistema este estable con un error del 2%:

${t_s(2\%)} \approx \frac{4}{\zeta \omega_n}$

## Sistema criticamente amortiguado

Posee dos polos iguales ubucados en el mismo punto del plano complejo para un sistema de segundo grado.

![image](https://github.com/user-attachments/assets/94be4310-4759-47fa-8da8-b2a78d1b504a)

### Respuesta de un sistema criricamente amortiguado

![image](https://github.com/user-attachments/assets/f3e1e762-f0b5-4650-8d3d-aa1cfe37a029)


Donde podemos hallar ts con un margen de error del 2% por medio de la siguiente formula:

$$t_s = \frac{5.8335}{\omega_n}$$

## Sistema Sobreamortiguado

Posee dos polos reales diferentes dentro de un sistema de segundo orden, donde ya no existe oscialciones.

![image](https://github.com/user-attachments/assets/e2ad81f2-e35b-44f4-9a22-05583b89ed27)

### Respeusta de un sistema sobreamortiguado 

![image](https://github.com/user-attachments/assets/7b9531b8-53e0-4f81-bb57-4fafe347abc6)

$$\tau_{eq} = \frac{2\zeta}{\omega_n}$$

# Sistema de orden Superior

Son sistemas de grado mayor a 2, debido a esro es posible descomponerlos en  polimonios de primer y segundo orden, por lo tanto los comportamineto seran combinaciones de funciones exponenciales y/o sinuosidales

## Polos dominantes

Dependiendo de su ubucacion de sistema tendra unos polos que predominaran en su comportamiento, donde los polos con parte real mas cerca al origen dominaran en el comportamiento del regimen transitorio del sistema.

Los otros polos estan alejados al menos una distancia 6 veces la ubicacion de los polos dominantes se considera insignificante efecto y se podra realizar una aproximacion.

## Retardo o tiempo muerto de un sistema 

En el dominio del tiempo el tiempo muerto se intertpreta como un corrimiento de la funcon hacia la derecha que indica que se demora en empenzar la funcion.

Al plicar la transformada de LaPlace a un desplazamineto en el tiempo lo que se obtien es un funcion exponencial.

## Ejemplo #1 :

### ¿Como controlar estos sistemas?

Para poder controlar estos sistemas sed debe saber que queremos lograr con la variable que se quire controlar, Comparar la varaiable que se quiere contolar con el valor deseado de las misma, a partir de resultado de la comparacion se toma una decision.

## Lazo cerrado 

Los sistemas de control de lazo cerrado son ampliamente utilizados en la variedad de industrias para regular y controlar procesos automatizados. Tambien es conocido como sistema de control realimentacion, utiliza una señal de retroalimentacion para comparar el resusltado deseado con el resultado actual y ajustar el proceso en consecuencia, permitiendo una mayor precision y estabilidad en comparacion con los sistemas de lazo abierto.

![image](https://github.com/user-attachments/assets/e471fd9e-ef97-4f93-95e4-af2f4e0552d2)


Este valor deseado se conoce como el Setpoint y sera el unico valor modificado en el sistema. La funcion de transferencia es esencial para analizar como se comporta el sistema ante diferentes entradas y perturbaciones. Para una comparacion profunda de como se determina y utiliza la funcin de transferencia en sistema de control.
