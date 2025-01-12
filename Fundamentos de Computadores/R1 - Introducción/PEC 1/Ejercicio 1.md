

## Dada la secuencia de bits A = 1011001011, indica a qué número decimal equivale según cada una de las interpretaciones siguientes:


### a) Se trata de un número binario entero representado en formato de complemento a 2. 

Primero de todo, analizamos el bit más significativo, que es el bit del extremo izquierdo. Vemos que es un 1, por lo que el resultado es un número negativo, y el resto contiene la magnitud.

Seguidamente, realizamos el complemento a 1 del número en binario, que consiste en cambiar los 0 por 1 y viceversa:

$$

\overline{011001011} = 100110100

$$

Una vez obtenida esta cifra, le sumamos 1, que nos da el siguiente resultado:

$$

\begin{array}{@{}c@{}c@{}} & 011001011 \\ + & \phantom{00000000}1 \\ \hline & 011001100 \\ \end{array}

$$

Que, si convertimos en decimal de base 10, nos da la siguiente cifra:

$$

1+4+16+32+256=309

$$

**Resultado:** Dado el signo negativo, el resultado es de -309
<br>
### b) Se trata de un número binario codificado en signo y magnitud en coma fija en un formato con 10 bits, de los cuales 4 son fraccionarios. 

Separamos el bit de signo que es 1 (bit del extremo izquierdo) y que indica signo negativo.

$$

1011001011 \to 011001011 

$$

El resto de bits 011001011 codifica la magnitud.

El valor decimal de la magnitud lo podemos conocer aplicando el TFN, teniendo en cuenta que los 5 últimos bits son los fraccionarios:

$$

\textrm{Parte entera} = 0110 =  0 \times 2^3 + 1 \times 2^2 + 1 \times 2^1 + 0 \times 2^0 = 6 

$$

$$

\textrm{Parte decimal} = 01011 = 0 \times {2^{0}} + 1 \times  {2^{−1}} + 0 \times  {2^{−2}} + 1 \times  {2^{−3}} + 1 \times  {2^{−4}} = \frac{11}{16}

$$

**Resultado:** El resultado decimal es de -6.6875.
<br>
### c) De este último formato (fraccionario de 10 bits con 4 bits para la fracción y codificación en signo y magnitud), ¿cuál es el rango de representación?

La parte entera del número puede variar de 0 a 11111, que es igual a 31 en decimal. La parte fraccionaria puede variar de 0 a 1111, que es igual a 15/16 en decimal.

**Resultado:** El rango de representación es de: $$[-31.9375 , 31.9375]$$

