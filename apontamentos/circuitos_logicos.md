# Circuitos Lógicos &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../README.md#indice)

Os circuitos lógicos têm como base as operações da Álgebra de Boole, e são fundamentais para o funcionamento de sistemas digitais. Estas operações simplificam a representação de estados em sistemas eletrónicos, limitando-os aos valores binários 0 e 1.

## Operações Lógicas Básicas

### 1. Operação OR (OU)
A operação OR, também conhecida como **soma lógica**, retorna o valor 1 quando **pelo menos uma das entradas** é 1.

- **Expressão matemática:** $S=A+B$
- **Descrição:** Retorna 1 se $A$ ou $B$ forem 1.

![image](https://github.com/user-attachments/assets/0dea5375-0be4-4af3-be42-6f2ce80f382f)


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

![image](https://github.com/user-attachments/assets/d2fbc75c-6639-40cd-a81d-0bff4a72e3f6)


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

![image](https://github.com/user-attachments/assets/80d6ff69-6136-46fc-992d-ceb71814d409)



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

![image](https://github.com/user-attachments/assets/1c615348-e34b-4c6e-9390-a7b0a9f84cdf)


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

![image](https://github.com/user-attachments/assets/b15b2ce4-5dac-4123-964d-a960cc28959c)


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

![image](https://github.com/user-attachments/assets/40648456-b29a-48ce-b3ba-f2e12e989e61)

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

![image](https://github.com/user-attachments/assets/341a0e0e-61d3-45f7-9d25-1d51f302bc4f)


**Tabela de Verdade:**

| A   | B   | $S=\neg(A\oplus B)$ |
| --- | --- | ------------------------ |
| 0   | 0   | 1                        |
| 0   | 1   | 0                        |
| 1   | 0   | 0                        |
| 1   | 1   | 1                        |

