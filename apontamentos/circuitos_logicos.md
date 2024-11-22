# Circuitos Lógicos &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../README.md#indice)

Os circuitos lógicos têm como base as operações da Álgebra de Boole, e são fundamentais para o funcionamento de sistemas digitais. Estas operações simplificam a representação de estados em sistemas eletrónicos, limitando-os aos valores binários 0 e 1.

## Operações Lógicas Básicas

### 1. Operação OR (OU)
A operação OR, também conhecida como **soma lógica**, retorna o valor 1 quando **pelo menos uma das entradas** é 1.

- **Expressão matemática:** $S=A+B$
- **Descrição:** Retorna 1 se $A$ ou $B$ forem 1.

![Imagem Porta Lógica OR](../img/gor.png)


**Tabela de Verdade:**
| A | B | S (A + B) |
|---|---|-----------|
| 0 | 0 |     0     |
| 0 | 1 |     1     |
| 1 | 0 |     1     |
| 1 | 1 |     1     |



### 2. Operação AND (E)
A operação AND, também conhecida como **produto lógico**, retorna o valor 1 quando **ambas as entradas** são 1.

- **Expressão matemática:** $S=A\cdot B$
- **Descrição:** Retorna 1 apenas se $A$ e $B$ forem ambos 1.

![Imagem Porta Lógica AND](../img/gand.png)


**Tabela de Verdade:**

| A   | B   | $S=A\cdot B$ |
| --- | --- | ------------ |
| 0   | 0   | 0            |
| 0   | 1   | 0            |
| 1   | 0   | 0            |
| 1   | 1   | 1            |



### 3. Operação NOT (NÃO)
A operação NOT, também conhecida como **negação** ou **complemento**, inverte o valor lógico da entrada.

- **Expressão matemática:** $S=\overline{A}$
- **Descrição:** Se $A=1$, então $S=0$ e vice-versa.

![Imagem Porta Lógica NOT](../img/gnot.png)


**Tabela de Verdade:**

| A   | $S=\overline{A}$ |
| --- | ---------------- |
| 0   | 1                |
| 1   | 0                |



## Portas Lógicas

### 1. Porta NAND
A porta NAND realiza uma operação **NOT AND**. A saída é 1 exceto quando **ambas as entradas** são 1.

- **Expressão matemática:** $S=\neg(A\cdot B)$
- **Descrição:** Retorna 1, a menos que $A$ e $B$ sejam ambos 1.

![Imagem Porta Lógica NAND](../img/gnand.png)


**Tabela de Verdade:

| A   | B   |  $S=\neg(A\cdot B)$ |
| --- | --- | ------------------------ |
| 0   | 0   | 1                        |
| 0   | 1   | 1                        |
| 1   | 0   | 1                        |
| 1   | 1   | 0                        |


### 2. Porta NOR
A porta NOR realiza uma operação **NOT OR**. A saída é 1 apenas quando **todas as entradas** são 0.

- **Expressão matemática:** $S=\neg(A+B)$
- **Descrição:** Retorna 1 apenas se $A$ e $B$ forem ambos 0.

![Imagem Porta Lógica NOR](../img/gnor.png)


**Tabela de Verdade:**

| A   | B   | $S=\neg(A+B)$ |
| --- | --- | ------------------ |
| 0   | 0   | 1                  |
| 0   | 1   | 0                  |
| 1   | 0   | 0                  |
| 1   | 1   | 0                  |


### 3. Porta XOR (OU Exclusivo)
A porta XOR retorna o valor 1 apenas se **um número ímpar de entradas** for 1.

- **Expressão matemática:** $S=A\oplus B$
- **Descrição:** Retorna 1 se $A$ e $B$ tiverem valores diferentes.

![Imagem Porta Lógica XOR](../img/gxor.png)

**Tabela de Verdade:**

| A   | B   | $S=A\oplus B$ |
| --- | --- | ------------- |
| 0   | 0   | 0             |
| 0   | 1   | 1             |
| 1   | 0   | 1             |
| 1   | 1   | 0             |


### 4. Porta XNOR
A porta XNOR é a **porta XOR com a saída invertida**. Retorna 1 se **ambas as entradas forem iguais**.

- **Expressão matemática:** $S=\neg(A\oplus B)$
- **Descrição:** Retorna 1 se $A$ e $B$ forem ambos 0 ou ambos 1.

![Imagem Porta Lógica XNOR](../img/gxnor.png)


**Tabela de Verdade:**

| A   | B   | $S=\neg(A\oplus B)$ |
| --- | --- | ------------------------ |
| 0   | 0   | 1                        |
| 0   | 1   | 0                        |
| 1   | 0   | 0                        |
| 1   | 1   | 1                        |

## Portas Lógicas Universais

As **portas lógicas universais** são portas lógicas que podem ser usadas para implementar qualquer outra porta lógica. As principais portas universais são:
### 1. Porta NAND

- **NOT**: Ligando ambas as entradas ao mesmo sinal.  
  - Fórmula: `NOT A = A NAND A`
 
![Pasted image 20241122160402](https://github.com/user-attachments/assets/65419577-32ab-4a04-92f9-7852b0145acd)

- **AND**: Porta NAND seguida de um inversor.  
  - Fórmula: `A AND B = (A NAND B) NAND (A NAND B)`
 
![Pasted image 20241122160517](https://github.com/user-attachments/assets/ae3519f5-3188-4686-bf8f-a578feaa39f4)

- **OR**: Combinando várias portas NAND.  
  - Fórmula: `A OR B = (A NAND A) NAND (B NAND B)`
 
![Pasted image 20241122160732](https://github.com/user-attachments/assets/aa714a38-d362-4850-9d1a-23e0f620dc3a)

### 2. Porta NOR 

- **NOT**: Ligando ambas as entradas ao mesmo sinal.  
  - Fórmula: `NOT A = A NOR A`
 
![Pasted image 20241122160922](https://github.com/user-attachments/assets/f6298b37-cef3-4892-b84e-9d924d4185af)

- **AND**: Combinando várias portas NOR.  
  - Fórmula: `A AND B = (A NOR B) NOR (A NOR B)`
 
![Pasted image 20241122161244](https://github.com/user-attachments/assets/aa751717-2fee-4aa0-ab83-8ff8815fc7cf)

- **OR**: Porta NOR seguida de um inversor.  
  - Fórmula: `A OR B = (A NOR A) NOR (B NOR B)`
 
![Pasted image 20241122161514](https://github.com/user-attachments/assets/cbadb9ab-7edd-4e15-bc54-2ff1f1e5604e)
