

## Realiza los cambios de base siguientes:

<br>
### a) Si B = -314 es un número decimal, represéntalo en complemento a 2 con el menor número de bits posible. 

Primero, obtenemos la representación binaria del valor absoluto de 314:

$$

314 = 0 \times 2^0 + 1 \times 2^1 + 0 \times 2^2 + 1 \times 2^3 + 1 \times 2^4 + 1 \times 2^5 + 0 \times 2^6 + 0 \times 2^7 + 1 \times 2^8 = 100111010

$$

Realizamos el complemento a 1 de la secuencia obtenida:

$$

\overline{100111010} = 011000101

$$

Y le sumamos 1 al resultado:

$$

\begin{array}{@{}c@{}c@{}} & 011000101 \\ + & \phantom{00000000}1 \\ \hline &  011000110 \\ \end{array}

$$

**Resultado**: Teniendo en cuenta que se ha de añadir un 1 a la izquierda para indicar el signo negativo, es la secuencia: **1011000110**

<br>
### b) Si C = 306 es un número octal, represéntalo en decimal. 

Si aplicamos la siguiente fórmula:

$$

C_{\text{decimal}} = C_0 \cdot 8^0 + C_1 \cdot 8^1 + C_2 \cdot 8^2 + \ldots + C_n \cdot 8^n

$$

Siendo C el decimal que buscamos, y C₀, C₁, C₂, ... Cₙ los dígitos del número en octal, si realizamos la operación:

$$

C_{\text{decimal}} = 6 \cdot 8^0 + 0 \cdot 8^1 + 3 \cdot 8^2 = 198

$$


**Resultado:** El número decimal que representa 306 en octal es el 198.

<br>
### c) Si D = 3A es un número hexadecimal, represéntalo en decimal. 

Si tenemos en cuenta la equivalencia entre los números decimales, binarios y hexadecimales de esta tabla:


| Decimal | Binario  | Hexadecimal |
| ------- | -------- | ----------- |
| 0       | 0000     | 0           |
| 1       | 0001     | 1           |
| 2       | 0010     | 2           |
| 3       | 0011     | 3           |
| 4       | 0100     | 4           |
| 5       | 0101     | 5           |
| 6       | 0110     | 6           |
| 7       | 0111     | 7           |
| 8       | 1000     | 8           |
| 9       | 1001     | 9           |
| 10      | 1010     | A           |
| 11      | 1011     | B           |
| 12      | 1100     | C           |
| 13      | 1101     | D           |
| 14      | 1110     | E           |
| 15      | 1111     | F           |


Vemos como el número dado corresponde a los dígitos 3 y 10, dado que A en hexadecimal corresponde a 10 en decimal.

Por tanto, dada la expresión:

$$D_{\text{decimal}} = D_0 \cdot 16^0 + D_1 \cdot 16^1 + D_2 \cdot 16^2 + \ldots + D_n \cdot 16^n$$

Teniendo en cuenta que D₀, D₁, D₂, ... Dₙ son los dígitos hexadecimales de derecha a izquierda, obtenemos la siguiente operación:

$$

D_{\text{decimal}} = 10 \cdot 16^0 + 6 \cdot 16^1 = 58

$$


**Resultado:** El valor 3A en Hexadecimal corresponde al número 58 decimal.
<br>
### d) Si E = -314 es un número decimal, represéntalo en signo y magnitud con el menor número de bits posible.

Obtenemos la secuencia decimal del valor absoluto de -314:

$$
314 = 0 \times 2^0 + 1 \times 2^1 + 0 \times 2^2 + 1 \times 2^3 + 1 \times 2^4 + 1 \times 2^5 + 0 \times 2^6 + 0 \times 2^7 + 1 \times 2^8 = 100111010
$$

Como resulta de un número negativo, hemos de añadir una cifra significativa al bit de mas a la izquierda, que será 0 si es positivo y 1 si es negativo.


**Resultado:** La representación binaria del número -314 es de **1100111010**