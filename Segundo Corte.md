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

## Dinamica de los sistemas de Segundo Orden

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

## Ejemplo #1 : $$G(s) = \frac{18}{s^2 + 2.4s + 9}$$
  $$\omega_n^2 = 9 \Rightarrow \omega_n = 3$$

$$K\omega_n^2 = 18 \Rightarrow K = \frac{18}{9} = 2$$

$$2\zeta\omega_n = 2.4 \Rightarrow \zeta = \frac{2.4}{2*3} = 0.4$$

$$t_p = \frac{\pi}{3\sqrt{1-0.4^2}} = 1.14_s$$

$$M_p = 100e\frac{-0.4\pi}{\sqrt{1-0.4^2}} = 25.38\%$$

$$t_s = \frac{4}{0.4*3} = 3.33_s$$

 ![image](https://github.com/user-attachments/assets/99f8e155-2529-4b3e-8836-a1e2bbef565b)

# ¿Como controlar estos sistemas?

Para poder controlar estos sistemas sed debe saber que queremos lograr con la variable que se quire controlar, Comparar la varaiable que se quiere contolar con el valor deseado de las misma, a partir de resultado de la comparacion se toma una decision.

## Lazo cerrado 

Los sistemas de control de lazo cerrado son ampliamente utilizados en la variedad de industrias para regular y controlar procesos automatizados. Tambien es conocido como sistema de control realimentacion, utiliza una señal de retroalimentacion para comparar el resusltado deseado con el resultado actual y ajustar el proceso en consecuencia, permitiendo una mayor precision y estabilidad en comparacion con los sistemas de lazo abierto.

![image](https://github.com/user-attachments/assets/e471fd9e-ef97-4f93-95e4-af2f4e0552d2)


Este valor deseado se conoce como el Setpoint y sera el unico valor modificado en el sistema. La funcion de transferencia es esencial para analizar como se comporta el sistema ante diferentes entradas y perturbaciones. Para una comparacion profunda de como se determina y utiliza la funcin de transferencia en sistema de control.

## Control ON-OFF

Este tipo de controlador, tambien llamado Todo o Nada, usa un algoritmo simple para solamente revisa la variable del proceso esta por encima o por debajo de un setpoint determinado.

En terminos practico, la variable manipuladad o la señal de control cambia entre totalmente OON o totalmente OFF, sin estados intermedios. Este tipo de accionamiento provoca un control muy impreciso de la variable de proceso.

![image](https://github.com/user-attachments/assets/09f2183b-57f2-4e95-bade-a864a249b350)


## Control Proporcional

Es la forma mas simple de control continuo que se puede utilizar en un sistema de lazo cerrado que corrigue el error entre una señal deseada y la señal real, aplicando una accion proporcional a ese error.
### ¿Como funciona?
El controlador proporcional genera una señal de control $u(t)$ que es directamente proporcionsl al error $e(t)$:

$$ u(t) = K_p*e(t)$$

$u(t)$: Señal de control que se envia al sistema

$e(t) = r(t) - y(t)$: Error, que es la diferencia entre la referencia  y la salida real.

$K_p$: Ganancia proporciona, una constante que determina que tan fuerte reacciona el sistema al error.

### ¿Que hace el Kp?
Si el Kp es bajo, la correcion es suave, pero lenta y puede haber error permanente, si el Kp es alto, la correccion es rapida, pero puede causar oscialciones o inestabilidad.

## Modelo de un sistema de primer orden

$$G(s) = \frac{K}{\tau s + 1}$$

K: Ganancia del sistema

$\tau$: Consate de tiempo

s: Varuable de Laplace

Utilizando agregando el control proporcional la ecuacion queda:

$$T(s) = \frac{K_p \cdot G(s)}{1 + K_p \cdot G(s)} = \frac{K_p \cdot K}{\tau s + 1 + K_p \cdot K}$$

# Estabilidad
## Teorema del valor final
Es una ecuacion bastante util en el analisis de sistemas y en la teoria dde control, donde nos indica cual es el valor final en el estado estacionario del sistema.

Cuando un sistema dinamico que se encuentra representado por nuna ecucion diferencial, llega al estado estacionario cuando el tiempo va para infinito, quiere decir qur los cambios en el sistema se vuelven nulos.

$$\lim_{s \to 0} \left[ sF(s) - f(0) \right]$$
$$\lim_{t \to \infty }[f(t)]$$

Una condicion es que el sistema debe ser estable. Si el sistema no es estable, el teorema del valor final no es estable 

### Analisis de estabilidad por el teorema de valor final

Para el analisis de estabilidad es necesario evaluar elvalor final de entrada y la de salida para establecer si estan limitadas de la misma manera.

Para la entrada:
$$\lim_{s \to 0} s \cdot \frac{A}{s} = A$$

En cuanto la salida de este es multiplicado por la entrada y se tambien se le aplica el limite.
## Analisis de establidad por ubicacion de polos
### Ubicacion de polos 
Las raices del poliimonio denominador de la funcion de transferencia, define los polos del sistemas. Dependiendo de la ubicacion de los polos de un sistema es posible determinar si un sistema es estable o no.

Si todos los polos del sistema estan ubicados en el semiplano  izquierdo, es decir si todos los polos tienen parte real negativa el sistema es estable.

Si por lo  menos un polo del sistema esta a la derecha del semiplano, el sistema es inestable.

## Criterio de Routh-Hurwitz
Es  una herramiemta analitica que se usa para determinar la estabilidad de un sistema sin tener que calcular los polos de su ecuacion caracteristicas, esta herramienta se utiliza con polimonios de grado superior.
### Condicion para estabilidad absoluta
Para que un sistema sea estable, todas las raices del polimonio caracteristico deben tener parte negativa. Y todos los elementos de la primera columna de la tabla de Routh tienen el mismo signo (y ninguno es cero).
### ¿Como se aplica?
1. Se forma la tabla de Routh, que es una especie de matriz organizada por filas que representa el polimonio.
2. A partir de los coeficientes del polimonio, se construye las filas sucesivas.
3. Se revisa la primera columna: Si todos los signos son positivos (o todos son negativos), es sistema es estabale. Si hay cambio de signo, hay raices en el simeplano derecho , lo que indica inestabilidad. 
### ¿Y si hay ceros o cambio de signo?
1. Si aparece  un cero en la primera columna, hay que aplicar un truco matematico (como derivar o usar una pequeña constante \varepsilon.
2. Si hay cambio de signo, cada cambio indica una raiz en el semiplano derecho.

### Diseño de control para que se estable 

Usamos un controlador porpocional $K_p$, Esto significa que simplemente estamos multiplicado la salida por un valor constante para tratar de controlar el sistema.

Cuando conectamos el comtrolador con la planta en un sistema en lazo cerrado, la funcio de transferencia pasa a:

$$T(s) = \frac{K_p \cdot G(s)}{1 + K_p \cdot G(s)}$$

Lo que nos interesa queda en el poliminio caracteristico, donde haremos la tabla con los coeficientes del poliminio. y gracias a ello en donde aparce la constante de porpocionalidad se pone mayor a 0, con el resultado se puede determinar que resultado de $K_p$ nos funciona para volver el sistema estable.
