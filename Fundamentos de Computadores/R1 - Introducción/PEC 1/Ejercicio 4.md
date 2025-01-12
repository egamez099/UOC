

## Dados los números binarios siguientes: $$ A = 0111010101    \ B = 1100010100 $$ Realiza las siguientes operaciones según el formato indicado en cada caso. Muestra los resultados únicamente en binario (no hay que hacer ninguna conversión a decimal) usando 10 bits, e indica y justifica en cada caso si se produce desbordamiento.
<br>
### a) A + B considerando que los números están codificados en signo y magnitud.

$$ \begin{array}{@{}c@{\;}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c} & 0 & 1 & 1 & 1 & 0 & 1 & 0 & 1 & 0 & 1 & \\ + & 1 & 1 & 0 & 0 & 0 & 1 & 0 & 1 & 0 & 0 & \\ \hline  1 & 0 & 0 & 1 & 1 & 1 & 0 & 1 & 0 & 0 & 1 & \end{array} $$

Vemos como sí se produce desbordamiento, al tener un resultado de 11 bits mayor que el de los sumandos que es de 10 bits.

**Resultado:** 10011101001  con desbordamiento.
<br>
### b) A - B considerando que los números están codificados en signo y magnitud.

$$ \begin{array}{@{}c@{\;}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c@{}c} & 0 & 1 & 1 & 1 & 0 & 1 & 0 & 1 & 0 & 1 & \\ - & 1 & 1 & 0 & 0 & 0 & 1 & 0 & 1 & 0 & 0 & \\ \hline  & 0 & 1 & 0 & 0 & 1 & 1 & 1 & 1 & 1 & 1 \end{array} $$

Al ser el resultado negativo, se añade un bit, que ocupa la posición 11, para indicación del signo.

Vemos como no se produce desbordamiento, al tener un resultado de 10 bits, que es igual al de los sumandos.

**Resultado:** 10100111111 sin desbordamiento.
<br>
### c) A + B considerando que los números están codificados en complemento a 2.

Primero calculamos el complemento a 1 de ambos números:

$$\overline{0111010101} = 1000101010 + 1 = 1000101011$$
$$\overline{1100010100} = 0011101011 + 1 = 0011101100$$

Y procedemos a sumarlos:

$$ 1000101011 + 0011101100 = 1100010111$$

Vemos como no se produce desbordamiento, al tener un resultado de 10 bits, que es igual al de los sumandos.

**Resultado:** El resultado es **01100010111** sin desbordamiento.
<br>
### d) A - B considerando que los números están codificados en complemento a 2.

Primero calculamos el complemento a 1 de ambos números:

$$\overline{0111010101} = 1000101010 + 1 = 1000101011$$
$$\overline{1100010100} = 0011101011 + 1 = 0011101100$$

Y procedemos a restarlos:

$$ 1000101011 - 0011101100 = 0100111111$$

Vemos como no se produce desbordamiento, al tener un resultado de 10 bits, que es igual al de los sumandos.

**Resultado:** El resultado es **0100111111** sin desbordamiento.