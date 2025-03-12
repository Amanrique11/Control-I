# 1.Sistemas mecanicos
## 1.1 Principio general de modelamineto 
$tasa de acumulacion\frac{masa }{energia}=flujo de \frac{masa }{energia}  entrada - flujo de \frac{masa }{energia}  salida$
## 1.2. Resorte
Se asumen que son resortes lineales, la fuerza externa aplicada y el desplazamiento estan relacionados por la constante de proporcionalidad.
$F=kx=k(x_1-x_2)$ de F= fuerza, k=constante de proporcionalidad , x= desplazamineto.


![Resorte](https://github.com/user-attachments/assets/b22260f0-2e53-466b-81e5-64a90d35f3dc)

Figura 1
## 1.3. Amortiguador 
Tiene un comportamiento linal, proporcional a la velocidad de desplazamiento. $F=bx'=b(x'_1-x'_2)$

![Amortiguador](https://github.com/user-attachments/assets/ecd2c904-0372-44e9-94bf-eca890b356e7)

FIgura 2
## 1.4. Tipos de friccion
### 1.4.1 Friccion en seco
Es aquella cuando se presenta cuando un cuerpo con una superfice no lubricada se desliza sobre otra superficie no lubricada.
Las cuales son: Friccion estatica, por deplazamiento y por rodamiento.
## 1.5. vibracion libre
Aun aplicando entrada durante un intervalo de tiempo definido es posible provocar un comportamiento oscilatorio en la variable de salida. Este movimiento periodico se conoce como vibracion libre.
# 2. Sistemas Electricos
## 2.1 Circutos RLC
Es un circuito que contiene recistencia (R), una inductancia (L) y una capacitancia (C), La resistencia representa la opocicion al flujo de corriente, la inductancia genera fuerza electromotriz proporcional a la variacion de corriente en el tiempo  y la capacitancia es la capacidad de almacenar energia en un campo  electrico.
## 2.2 Clasificacion de circuitos RLC
### 2.2.1 Circuito RLC en Serie
Todos los componentes estan conectados en una misma trayectoria, por lo que la misma corriente fluye a traves de todos ellos, Por lo contrario el voltaje se reparte entre los componentes.
### 2.2.2 Circuito RLC en Paralelo
Cada componente está conectado de manera independiente a la fuente de alimentación, lo que significa que la corriente puede tomar diferentes caminos.
## 2.3 Modelamiento en circuiros RLC
En en modelamiento en circuitos electricos, se analiza por medio de las leyes de Kirchoff, ya se por mallas o por nodos, Por mallas nos enfocamos en que los voltajes en la malla sea 0, y por nodos nos enfocamos en las corrientes que entran a un nodo, y esta debe ser tambien igual a 0.
## 2.4 Amplificadores operacionales
Es un circuito integrado que permite hacer gran variedad de circuitos utiles. Desde comparador de voltajes, un amplificador de señal, hacer operaciones aritmeticas y filtar señales. Los amplificadores estan compustos por una gran cantidad de transistores internamente que perimite controlar corrientes y tensiones, para darle sus caracteristicas electricas.

Para hacer su modelacion debemos tener encuenta que en sus etradas no hay corriente ademas de que el volatje de las entradas son las mismas, y para facilitar el modelamiento se analiza por medio de las leyes de kirchoff por nodos.
# 3.  Transformada de Laplace
## 3.1.  ¿Que es la transformada de Laplace?
Es una tecnica para resolver ecuaciones diferenciales con condiciones iniciales, por medio de un cambio de espacio geometrico del dominio del tiempo hacia el dominio de la frecuecia compleja.
A continuacion vemos como es ecuacion de la transformada:
$$\mathcal{L}\{f(t)\}=\int_0^{+\infty} e^{-s t} f(t) d t$$
## 3.2. Transformada inversa de Laplace
La trasnformada iversa nos ayuda a pasar del dominio de la frecuencia compleja a el diminio del tiempo para que nuestro reltado se pueda manejar mas facil.
Si las funciones son simples utilizar la tabla de transformadas. Si las funciones son una combinacion o una composicion de varias funciones se debe realizar una expansion de fracciones parciales para obtner una suma de funciones mucho mas simple que se puedan encontrar en las tablas de transfromadas.
$$f=\mathcal{L}^{-1}(F)$$
## 3.3 Propiedades de la transformada de Laplace
### 3.3.1 Propiedad de la linealidad de la transformada de Laplpace
La transformacion de Laplace es lineal, esto es, dadas dos funciones f, g ∈ E se verifica.
$\mathcal{L}\left[C_1 f(t)+C_2 g(t)\right]=C_1 \mathcal{L}[f(t)]+C_2 \mathcal{L}[g(t)]$ donde C1 y C2 pertenece a los relaes.
### 3.3.2 Proppiedad de cambio de escala
Sea f(t) ∈ E. La funcion g(t) = f(αt) tambien pertenece a E y se verifica.
$$\mathcal{L}[g(t)] \equiv G(s)=\frac{1}{\alpha} F\left(\frac{s}{\alpha}\right)$$
### 3.3.3 Propiedad de desplazamiento en frecuencia
Sea f(t) ∈ E. La funcion $g(t)=e^{\omega t} f(t)$ tambien pertenece a E y se verifica.
$$\mathcal{L}\{f(t)\}=\int_0^{+\infty} e^{-s t} f(t) d t$$
### 3.3.4 Propiedad de desplazamiento en el tiempo
Sea f(t) ∈ E. La funcion $g(t)=f(t-\widetilde{T}) u(t-\widetilde{T})$ tambien pertenece a E y se verifica.
$\mathcal{L}[g(t)] \equiv G(s)=e^{-T s} F(s)$
![ecuacion](https://github.com/user-attachments/assets/a43b0964-61cb-4715-9590-31ac21478e3d)
## 3.4. Transformadas 
### 3.4.1 Transformada de una funcion
$\mathcal{L}[f(t)]=F(s)$
### 3.4.2 Transformada de la derivada
$\mathcal{L}[f'(t)]=sF(s)-f(0)$

$\mathcal{L}[f''(t)]=s^{2}F(s)-sf'(0)$

$\mathcal{L}[f^{n}(t)]=s^{n}F(s)-s^{n-1}f(0)-...-sf^{n-1}-f^{n}$
### 3.4.3 Transformada de la integral
$\mathcal{L}[\int f(t)]=\frac{1}{s}F(s)$
### 3.4.4 Tabla de transformadas
![Tabla de transformadas](https://github.com/user-attachments/assets/740994db-c24b-4de1-8525-7f45ccda0fd7)
Figura 1. Tabla de las transformadas
#  Ejercicios 
## 📚 1. Calcular la transformada de Laplace de $f(t)=2t^{3}+e^{5t}+\sin{3t}$
$\mathcal{L}[f(t)]=2\mathcal{L}[t^{3}]+\mathcal{L}[e^{3t}+4\mathcal{L}[sin{3t}]$

$\mathcal{L}[f(t)]=2\frac{6}{s^{4}}+\frac{1}{s-5}+4\frac{3}{s^{2}+9}$
## 📚 2. Hallar $f(t)$  de $\frac{8s}{(s^{2}+1)^{2}}$
$\mathcal{L}^{-1}[\frac{8s}{(s^{2}+1)^{2}}]=8\frac{1}{s^{2}+1}\frac{s}{s^{2}+1}$

$\mathcal{L}^{-1}[\frac{8s}{(s^{2}+1)^{2}}] = 8sin{t}cos{t}$
# 4.Funcion de Transferencia 
## 4.1 Definicion y conceptos clave:
la funcion de transferencia describe la relacion entre la entrada y la salida de un sistema lineal en el dominio de Laplace. Se expresa como:

$$G(s)=\frac{Y(s)}{U(s)}$$

## 4.2 Clasificacion de las funciones de transferencia
1. Impropias: Grado de numerador $$N(s)$$ > grado del denominador $$D(s)$$.
2. Estrictamente propias: Grado $$D(s)$$ > grado de $$N(s)$$.
3. Bipropias: Grados iguales en $$N(s)$$ y $$D(s)$$.
## 4.3 Zeros y Polos
Zeros: Son los valores de $$s$$ que hacen cero el numerador $$N(s)$$ de la funcion de transferenci $$G(s)$$
Polos: Son los valores de $$s$$ que hacen cero el denominador $$D(s)$$ de $$G(s)$$, lo que hace la funcion de transferencia tienda a infinito.
## 4.4 Representacion en el plano complejo
Eje real: Indica componentes relacionadas con la rapidez de la repuesta del sistema.
*Polos en el semiplano izquierdo: La funcion de transferencia es estable.
*Polos en el semiplano derecho: La funcion es inestable.
Eje imaginario: Indica componentes oscilatorias de la respuesta.
