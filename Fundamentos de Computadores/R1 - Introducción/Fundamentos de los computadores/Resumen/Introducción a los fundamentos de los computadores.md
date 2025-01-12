
<br>

## 1.  El estudio de los fundamentos de los computadores
<br>
> **PLC:** Siglas de "programmable logic controller": Equipamiento electrónico programable diseñado para controlar sucesos secuenciales.


**Electrónica analógica:** Las señales varían de forma *contínua*. Se registra cualquier valor de tensión dentro de unos márgenes.

**Electrónica digital:** Basada en señales sobre las que sólo se identifica un *conjunto finito* de valores (0 y 1), por lo que solamente se registran los diferenciales de potencial entre el mas alto y el mas bajo.

Todas las señales han de estar *codificadas* de forma adecuada, para poder manipularlas en 0s y 1s lógicos.

<br>
![[Pasted image 20240219175734.png]]

<br>
### 1.1 Codificación de la información y sistemas digitales

<br>
Cada elemento tendrá una representación y otra según el conjunto de reglas de codificación; por lo que el sistema de representación determinará la codificación de la información.

Si trabajamos en un sistema que manipula solamente dos posibles valores, (los dos niveles de tensión), tendremos que codificar la información en *base 2*.

En la electrónica digital las señales representan números, y en las analógicas la información está contenida en ondas.


![[Drawing 2024-02-19 18.04.21.excalidraw]]

<br>

## 2.  La evolución de los computadores


| Autor            | Periodo     | Descripción                                                                                                                                                                                                                                                                                                                       |
| ---------------- | ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charles Babbage  | 1791 - 1871 | Concibe la **Máquina analítica**. Incorpora el concepto de máquina dirigida por un programa externo. Incluía una memoria mecánica, una unidad de procesamiento, una unidad de control (formada por cilindros), una entrada de datos (similar a las tarjetas perforadas) y salida por impresión (similar a la máquina de escribir) |
| Herman Hollerith | 1860 - 1929 | Gracias al descubrimiento de la energía eléctrica, se desarrollan máquinas electromecánicas. Considerado el primer informático en hacer un tratamiento automatizado de la información.                                                                                                                                            |
| Konrad Zuse      | 1910 - 1995 | Z1 -> Memoria mecánica binaria. Z2 -> Realizaba el procesamiento a partir de relés y mejoraría a la Z3 y Z4.                                                                                                                                                                                                                      |
| George Stibitz   | 1904 - 1995 | Computadores de relés para laboratorios Bell                                                                                                                                                                                                                                                                                      |
| Howard Aiken     | 1900 - 1973 | Serie Mark para la Universidad de Harvard -> Primeras máquinas con propósito comercial.                                                                                                                                                                                                                                           |

<br>

### 1ª generación (1940 - 1955)

### 2ª generación (1955 - 1965)

### 3ª generación (1965 - 1970)

### 4ª generación (1970 - Current)



## 3. Computadores digitales en la actualidad


**Computador digital:** Sistema que trabaja con datos numéricos; cuya interpretación depende del formato en que se esté trabajando. Normalmente en sistema de numeración en base 2 -> Señales binarias en las que solo podemos identificar dos valores distintos.

![[Pasted image 20240219181813.png]]


- **Dispositivo de entrada y salida:** Se trata de elementos de conversión de la información entre el sistema analógico del exterior y el sistema digital que utiliza la CPU. Almacenan información digital que el procesador puede recuperar.

- **Procesador:** Constituída por una *Unidad Central de Proceso* y la memoria asociada. Se encarga de procesar los datos según el programa establecido. A su vez está formada por la Unidad de Control y Unidad de Proceso (o camino de datos).
	- **Unidad de Proceso:** Reúne los recursos de cálculo.
	- **Unidad de Control:** Encargada de dar las órdenes en la secuencia correcta a la unidad de proceso para realizar las operaciones que establece el programa en ejecución.

### 3.1 Arquitectura de Vonn Newman


![[Pasted image 20240219182456.png]]

Se caracteriza por el hecho de que tanto los datos como el programa se almacenan en la memoria principal; directamente unida con la CPU.

#### Características:

- **Programa almacenado:** Tanto los datos como las instrucciones del programa residen en la memoria principal. Conlleva dos consecuencias:
	1. Dota al computador de amplia generalidad.
	2. Existe un cuello de botella en la comunicación entre la CPU y la memoria, ya que impacta directamente en el rendimiento de la máquina.

- **Unidad de control simple:** La *Unidad de Control* no tiene que ejecutar todo el programa, sino que se encarga de únicamente ejecutar de forma iterativa las instrucciones.


### 3.2 Arquitectura Harvard

![[Pasted image 20240219183132.png]]

Se separa la memoria de los datos de la memoria de las instrucciones del programa a ejecutar. 

#### Características:

- Corrije la limitación del acceso a memoria, ya que permite realizar operaciones en la memoria de los datos mientras que se accede a la memoria de las instrucciones.

- Limita la posibilidad de *automodificar* los programas: 


>  Código que altera sus propias instrucciones mientra este es ejecutado con el objetivo de reducir la longitud del camino de instrucciones y así mejorar el rendimiento y reducir código similar, simplificando así el mantenimiento. 
 