# Comparadores &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

A função básica de um comparador é comparar as magnitudes de dois números binários para determinar a relação comparativa entre eles. 

## Comparador Simples

Na sua forma mais simples, um circuito comparador determina se dois números são iguais. 
A porta XOR pode ser usada como um comparador básico porque a sua saída é nível 1 se os dois bits de entrada forem diferentes e é 0 se os bits de entrada forem iguais.

![Pasted image 20241208103434](https://github.com/user-attachments/assets/bd7b290b-dbff-48a8-813a-196984426d39)

### Dois Bits
Para comparar números binários com dois bits cada um, é necessário mais uma porta XOR. 
Os dois bits menos significativos (LSBs) dos dois números são comparados pela porta G1 e os dois bits mais significativos (MSBs) são comparados pela porta G2. 
Se os dois números forem iguais, os bits correspondentes são iguais, sendo a saída de cada porta XOR nível zero. Se o conjunto correspondente de bits não forem iguais, a saída da porta XOR é nível 1.

![Pasted image 20241208103513](https://github.com/user-attachments/assets/81082822-4013-486d-8715-ac25678af895)

## Exemplo
Considerando os seguintes conjuntos de números binários e o circuito comparador mostrado na figura, determine a saída do circuito para cada conjunto.
- (a) 10 e 10
- (b) 11 e 10

![Pasted image 20241208103609](https://github.com/user-attachments/assets/57aa5a14-fabb-4b1b-b0ba-497bf476ce7c)

- (a) A saída é nível 1 para as entradas 10 e 10.
- (b) A saída é nível 0 para as entradas 11 e 10.


## Comparador completo

Além da saída de igualdade, muitos CIs comparadores têm saídas adicionais que indicam qual dos dois números binários comparados é maior. 
Assim, existe uma saída que indica quando o número A é maior que o número B (A > B) e uma saída que indica quando o número A é menor que o número B (A < B), como mostra o símbolo lógico para um comparador de 4 bits.

![Pasted image 20241208103718](https://github.com/user-attachments/assets/2aac120e-a080-4ae8-8df7-013719ddb060)

Para determinar uma desigualdade dos números binários A e B, temos que examinar primeiro o bit mais significativo de cada número. As seguintes condições são possíveis: 
1. Se A3 = 1 e B3 = 0, o número A é maior que o número B. 
2. Se A3 = 0 e B3 = 1, o número A é menor que o número B. 
3. Se A3 = B3 , então temos que examinar a desigualdade do próximo bit da posição mais inferior. 
Essas três operações são válidas para a posição de cada bit nos números.

### Exemplo

Determine as saídas A = B, A > B e A < B para os números de entradas mostrados no comparador visto na Figura:

![Pasted image 20241208103834](https://github.com/user-attachments/assets/67d94d5e-f2fb-4135-bab4-e266ff6a0091)

- O número nas entradas A é 0110 e o número nas entradas B é 0011.
- A saída A > B é nível ALTO e as outras saídas são nível BAIXO.
