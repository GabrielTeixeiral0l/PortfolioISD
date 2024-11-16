## exercício 1

1. Consideremos um laboratório que tem armazenado produtos químicos. Nesse armazém, sabemos que existem quatro produtos químicos. Desses, o Produto A, Produto B, Produto C e Produto D devem ser guardados em dois depósitos. Nesse laboratório também se sabe que de vez em quando é necessário mover um ou mais produtos de um depósito para o outro, assim como, atendendo à natureza dos produtos, é perigoso guardar o Produto B e o Produto C juntos, a não ser que o Produto A esteja no mesmo depósito. Para além disso, sabe-se também que é perigoso guardar o Produto C e o Produto D juntos se o Produto A não estiver no depósito. Escreva uma expressão para uma função, S, tal que S = 1 sempre que exista uma combinação perigosa em qualquer dos depósitos. 

### Análise

Produtos:
A B C D
Depósitos:
- 2 depósitos
- 0 corresponde a um depósito e 1 a outro
Condições:
PRIOBIDO
- B e C juntos 
- C e D JUNTOS
AMBOS SEM A

### Tabela de verdade

| A   | B   | C   | D   | S   | TENTATIVA 1 | TENTATIVA 2 |
| --- | --- | --- | --- | --- |:-----------:|:-----------:|
| 0   | 0   | 0   | 0   | 0   |             |             |
| 0   | 0   | 0   | 1   | 0   |             |             |
| 0   | 0   | 1   | 0   | 0   |             |             |
| 0   | 0   | 1   | 1   | 1   |             |             |
| 0   | 1   | 0   | 0   | 0   |             |             |
| 0   | 1   | 0   | 1   | 0   |             |             |
| 0   | 1   | 1   | 0   | 1   |             |             |
| 0   | 1   | 1   | 1   | 1   |             |             |
| 1   | 0   | 0   | 0   | 1   |             |             |
| 1   | 0   | 0   | 1   | 1   |             |             |
| 1   | 0   | 1   | 0   | 0   |      x      |             |
| 1   | 0   | 1   | 1   | 0   |      x      |             |
| 1   | 1   | 0   | 0   | 1   |             |             |
| 1   | 1   | 0   | 1   | 0   |      x      |             |
| 1   | 1   | 1   | 0   | 0   |      x      |             |
| 1   | 1   | 1   | 1   | 0   |             |             |


### TENTATIVA 1 (LOGICLY)

#### primeira condição

![Pasted image 20241116133440](https://github.com/user-attachments/assets/f0d03c60-5114-4543-95fa-1f052ca4357e)


### CONCLUSÃO

![Pasted image 20241116140836](https://github.com/user-attachments/assets/f26d39a1-f660-4daa-a595-c4d5ad30c5cb)


### TENTATIVA 2 (EXPRESSÃO)

#### primeira condição (verificar se B e C estão no mesmo depósito)

$\overline{B\oplus C}$

![Pasted image 20241116144219](https://github.com/user-attachments/assets/643b588f-5638-49e5-b1ec-3ed4a9df0769)

#### segunda condição (verificar se A B e C são iguais)

$(\overline{A\oplus B})(\overline{B\oplus C})$

![Pasted image 20241116144416](https://github.com/user-attachments/assets/e47d28b8-40fc-4bd7-8369-ad8a79de61c3)

#### Junção das duas condições
 
para a junção das duas condições tive de fazer uma pequena alteração na segunda expressão, para que o valor caso fossem iguais fosse 0.

$\overline{(\overline{A\oplus B})(\overline{B\oplus C})}$

$\overline{(\overline{A\oplus B})(\overline{B\oplus C})}(\overline{B\oplus C})$

![Pasted image 20241116144618](https://github.com/user-attachments/assets/06aad27e-9e90-4101-a4fa-d775afc5a267)

terceira condição (verificar se C e D estão no mesmo depósito)

$\overline{C\oplus D}$

![Pasted image 20241116145945](https://github.com/user-attachments/assets/175b9d39-d4dd-41b0-a1f3-7c0fb58bfe72)

quarta condição (verificar se A C e D são iguais)

$(\overline{A\oplus C})(\overline{C\oplus D})$

![Pasted image 20241116152225](https://github.com/user-attachments/assets/3719a910-8d6c-4cc2-bad6-4bdaf757a925)

Junção das duas condições (terceira e quarta)

$\overline{(\overline{A\oplus C})(\overline{C\oplus D})}(\overline{C\oplus D})$

![Pasted image 20241116152628](https://github.com/user-attachments/assets/7a4aae77-9ffd-4bd9-a267-58ed81e39567)

CONCLUSÃO

$\overline{(\overline{A\oplus B})(\overline{B\oplus C})}(\overline{B\oplus C})+\overline{(\overline{A\oplus C})(\overline{C\oplus D})}(\overline{C\oplus D})$

![Pasted image 20241116153045](https://github.com/user-attachments/assets/b024255b-359c-434d-8d6f-6f33773cb688)

Na segunda tentativa, consegui completar o desafio ao mudar a minha forma de pensar. Na primeira tentativa, foquei-me numa parte envolvendo apenas as entradas A, B e C, resolvendo no **Logicly**. Contudo, após alguns passos, percebi que estava a avançar de forma automática, recorrendo à tentativa e erro. Na segunda tentativa, dividi o problema em partes mais pequenas, trabalhei sempre apenas com dois valores de entrada de cada vez. Além disso, em cada passo, fui escrevendo a expressão lógica correspondente, o que me ajudou a estruturar melhor o raciocínio.


## exercício 2

2. Considere três interruptores, x, y e z. X = 1 representa a condição “interruptor x ligado”, e X = 0 representa a condição “interruptor x desligado”. Da mesma forma, as variáveis Y e Z estão associadas às posições dos interruptores y e z, respetivamente. Escreva uma expressão booleana para uma função S, de modo que a alteração do estado de um interruptor, independentemente dos outros, vá provocar a mudança do valor da função.

### Análise 
- 3 variáveis 

### Primeiro passo (utilizar apenas X e Y)

Com dois interruptores, o que tinha que acontecer era, se a luz tivesse desligada ao pressionar qualquer um dos interruptores a luz tinha que apagar e vice-versa.


#### Tabela

| iterações | interruptor 1 | interruptor 2 | luz |
| :-------: | :-----------: | :-----------: | :-: |
|     1     |       0       |       0       |  0  |
|     2     |       0       |       1       |  1  |
|     3     |       1       |       1       |  0  |
|     4     |       0       |       1       |  1  |

tabela xor

|  X  |  Y  | S= ${X\oplus Y}$ |
| :-: | :-: | :--------------: |
|  0  |  0  |        0         |
|  0  |  1  |        1         |
|  1  |  0  |        1         |
|  1  |  1  |        0         |


${X\oplus Y}$

![Pasted image 20241116185306](https://github.com/user-attachments/assets/333ff647-5073-48e8-967b-2cb8374596f3)

### Segundo passo (Adicionar o Z)

Para adicionar a entrada Z, percebi logo que podia adicionar outro xor com entradas o resultado de ${X\oplus Y}$ e ${ Z }$, testei no logicly e resultou
${X\oplus Y \oplus Z}$

![Pasted image 20241116185411](https://github.com/user-attachments/assets/77c232d5-d6e6-4766-a84a-3677762ee48b)
