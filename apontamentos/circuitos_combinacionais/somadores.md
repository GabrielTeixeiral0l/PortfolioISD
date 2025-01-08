# Somadores &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

Os somadores são importantes em computadores e também noutros tipos de sistemas digitais nos quais dados numéricos são processados. 
Uma compreensão da operação básica de um somador é fundamental no estudo de sistemas digitais.
### Meio-Somador

Relembrar as regras básicas para a adição binária... 
- As operações são realizadas por um circuito lógico chamado de meio-somador. 
- O meio-somador aceita dois dígitos binários nas suas entradas e produz dois dígitos binários nas suas saídas, um bit de soma e um bit de carry.
- Um meio-somador **soma dois bits e produz um resultado (soma)** e um **carry de saída**.

![Pasted image 20241208102018](https://github.com/user-attachments/assets/2932020f-1c8f-48ea-950b-56c1cd0cccd5)

#### Tabela de Verdade
Lógica do Meio-Somador: A partir da operação do meio-somador expressa na Tabela, podemos deduzir expressões para a soma (resultado) e para o carry de saída como funções das entradas. Observe que o carry de saída (Cout) é 1 apenas quando A e B são 1s; portanto, Cout pode ser expresso como uma operação AND entre as variáveis de entrada.

![Pasted image 20241208102101](https://github.com/user-attachments/assets/9c82c1fb-915e-4c11-9ab2-5013711fc103)

![Pasted image 20241208102109](https://github.com/user-attachments/assets/d6ae354e-3b1b-413c-99d4-eefd57f447aa)


#### Diagrama Lógico de um Meio-somador

![Pasted image 20241208102122](https://github.com/user-attachments/assets/cbf431b7-ec7b-4a63-89ee-21b71e325627)

### Somador Completo

A segunda categoria de somadores é o somador-completo. 
O somador-completo aceita dois bits de entrada e um carry de entrada, e gera uma saída de soma e um carry de saída. 
A diferença básica entre um somador-completo e um meiosomador é que o somador-completo aceita um carry de entrada.

Um somador-completo tem um carry de entrada, enquanto que um meio-somador não tem.

![Pasted image 20241208102252](https://github.com/user-attachments/assets/4bcd1b0c-c547-432b-b2c6-cc07eb49a132)

#### Tabela de Verdade

![Pasted image 20241208102419](https://github.com/user-attachments/assets/f7f5d604-0950-489c-b3b6-6795e2024850)


#### Circuito Lógico do Somador-Completo
O somador-completo soma os dois bits de entrada e o carry de entrada. A partir do meiosomador sabemos que a soma dos bits de entrada A e B é a EX-OR

![Pasted image 20241208102525](https://github.com/user-attachments/assets/b8d07075-1dd8-4984-af64-f983e0066235)

#### Somador-completo implementado com meio-somadores.

![Pasted image 20241208102552](https://github.com/user-attachments/assets/252db53c-b5b3-4200-93ff-145148fa24ee)

![Pasted image 20241208102617](https://github.com/user-attachments/assets/5cfadf51-0e47-4c3d-b7e5-16d6c250a4d0)


### Resumo

![Pasted image 20241208102646](https://github.com/user-attachments/assets/77fa118b-1814-49d0-8ac0-6b29a797b70f)


### Exemplo

Para cada um dos três somadores-completos na Figura, determine as saídas para as entradas mostradas

![Pasted image 20241208103948](https://github.com/user-attachments/assets/8807cd17-b7b6-4820-947b-2f2b8a3b74e0)

![Pasted image 20241208104002](https://github.com/user-attachments/assets/831de1b5-8f97-4ea1-9557-4b3d17932a67)

![Pasted image 20241208104010](https://github.com/user-attachments/assets/d1176509-55db-4616-8fab-749da2d44c82)

![Pasted image 20241208104018](https://github.com/user-attachments/assets/653b9825-7540-4d58-9598-2618fd047749)


# Somadores Binários Paralelos

Dois ou mais somadores-completos podem ser conectados para construir somadores binários paralelos. 
Um único somador-completo é capaz de somar dois números de 1 bit e um carry de entrada.
Para somar números binários com mais de 1 bit, temos que usar somadores-completos adicionais. Quando um número binário é somado a outro, cada coluna gera um bit de soma e um bit de carry (que pode ser 1 ou 0) para a próxima coluna à esquerda, conforme ilustrado a seguir com números de dois bits.

![Pasted image 20241208102831](https://github.com/user-attachments/assets/e065e9b7-0d1e-4c26-89c5-b4beac719ed8)


Para somar dois números binários, é necessário um somadorcompleto para cada bit do número. • Assim, para números de dois bits, são necessários dois somadores; para números de 4 bits, são usados quatro somadores; e assim sucessivamente.

A saída de carry de cada somador é conectada à entrada de carry do próximo somador de maior ordem, conforme mostra a figura para um somador de dois bits. • Atenção que um meio-somador pode ser usado na posição menos significativa ou um somador-completo com a entrada de carry colocada em 0 (GND) porque não existe entrada de carry na posição do bit menos significativo.

![Pasted image 20241208102905](https://github.com/user-attachments/assets/eb7e7a85-16c1-494e-a77c-c0028b599ce1)

Nota: Na Figura o bit menos significativo (LSB) dos dois números são representados por A1 e B1 . Os próximos bits de ordem maior são representados por A2 e B2 . E os três bits de soma são Σ1 , Σ2 e Σ3 . O carry de saída do somadorcompleto mais à esquerda se torna o bit mais significativo (MSB) do resultado (soma), Σ3 .

### Exemplo:

Determine a soma gerada pelo somador paralelo de 3 bits visto na figura e mostre os carries intermediários quando os números binários 1010 e 011 são somados.

![Pasted image 20241208104120](https://github.com/user-attachments/assets/604fb120-d977-4a45-88a9-a7e22640e14c)

![Pasted image 20241208104154](https://github.com/user-attachments/assets/a8792060-6f9a-496e-8fea-e4f24a78c4f8)

**Os LSBs dos dois números são somados no somador-completo mais à direita. Os bits do resultado e os carries intermediários são indicados em cinza.**
## Somadores Paralelos de Quatro Bits
Um grupo de quatro bits é denominado de **nibble**. 
Um somador paralelo de 4 bits básico é implementado com quatro estágios de somadores-completos como mostra a figura.

![Pasted image 20241208103127](https://github.com/user-attachments/assets/8f69d7fd-372b-4e60-be6d-a8ce8b6097dd)

Os bits LSB (A1 e B1 ) em cada número são somados pelo somadorcompleto mais à direita; os bits de ordem mais alta são inseridos sucessivamente nos somadores de ordem mais alta, com os MSBs (A4 e B4 ) em cada número inseridos no somador-completo mais à esquerda. • A saída de carry de cada somador é conectada à entrada de carry para o próximo somador de ordem mais alta conforme indicado. Esses são denominados de carries internos.


De acordo com as folhas de dados dos fabricantes, a entrada denominada de C0 é o carry de entrada do bit menos significativo do somador; no caso do quatro bits, C4 é o carry de saída do bit mais significativo do somador; e ∑ 1 (LSB) até ∑ 4 (MSB) são as saídas do resultado (soma).
Em termos do método usado para operar com carries em somadores paralelos, existem dois tipos: o somador com carry ondulante (ripple carry) e o somador com carry antecipado (lookahead carry).

### Tabela-verdade para cada estágio de um somador paralelo de 4 bits

![Pasted image 20241208103224](https://github.com/user-attachments/assets/67d4cf3b-2063-4b7d-806f-e5b9eec7b7a7)


### Somadores Paralelos de Quatro Bits (74LS283)
Um exemplo de um somador paralelo de 4 bits que é comercializado é o CI 74LS283. 
VCC é o pino 16 e GND é o pino 8, que é uma configuração padrão. 
O digrama de pinos e o símbolo lógico para o dispositivo são mostrados na figura (com os números os pinos em parênteses no símbolo lógico).

![Pasted image 20241208103340](https://github.com/user-attachments/assets/bfd351b0-7ef5-4574-aadc-3f46ddf9ae54)
