

## Dado el número decimal fraccionario 27,35 se pide:
<br>
### a) Representa este número en binario con una codificación en coma fija en un formato con 8 bits, de los cuales 3 son fraccionarios. Usa aproximación por redondeo.

Primero separamos la parte entera de la decimal; que viene a ser:

$$ \textrm{Parte entera} = 27 $$
$$ \textrm{Parte decimal} = 0,35 $$

Seguidamente, realizamos la conversión a binario de la parte entera:

$$ 27_{\text{10}} = 1 \times 2^0 + 1 \times 2^1 + 0 \times 2^2 + 1 \times 2^3 + 1 \times 2^4 = 11011_{\text{2}} $$

Para la parte decimal, convertimos la parte fraccionaria 0,35 a binario utilizando aproximación por redondeo y limitándonos a 3 bits fraccionarios:

$$ 0,35 \times 2 = 0,7 \to \text{Bit mas significativo = 0} $$
$$ 0,7 \times 2 = 1.4 \to \text{Bit mas significativo = 1} $$
$$ 0,4 \times 2 = 0,8 \to \text{Bit mas significativo = 0} $$

Por lo que el redondeo en binario de la parte fraccionaria resulta en 010

**Resultado:** La representación es de **11011010**.
<br>
### b) ¿Se produce algún error en la representación? En caso afirmativo, indica el valor decimal de este error

Sí, se produce un error, ya que el número obtenido, 11011010, equivale al siguiente número decimal teniendo en cuenta la posición de la coma flotante:

$$ \text{Parte entera = 11011}$$
$$ \text{Parte decimal = 101} $$

Convertimos estos valores:

$$ 11011_{\text{2}} = 1 \times 2^0 + 1 \times 2^1 + 0 \times 2^2 + 1 \times 2^3 + 1 \times 2^4= 27_{\text{10}}$$

$$ 010_{\text{2}} = 0 \times 2^{−1} + 1 \times 2^{−2} + 0 \times 2^{−3} = \frac{1}{4}_{\text{10}} = 0,25_{\text{10}} $$

Por tanto, el resultado de la conversión es de 27,25.

El error, por tanto, es el resultado de restar la cifra original por la cifra obtenida:

$$ 27,35 - 27,25 = 0,1 $$

**Resultado:** El error obtenido es de **0,1**