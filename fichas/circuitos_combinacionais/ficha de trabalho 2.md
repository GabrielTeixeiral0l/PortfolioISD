# Ficha de trabalho 2 - Somadores e Comparadores &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

1.Quais são as saídas de um somador-completo para A = 1, B = 1 e Cin = 1?

1 + 1 +1 = 1 C_out de 1

soma = 1
C_out = 1

2.Determine a soma (∑) e o carry de saída (Cout) de um meio-somador para cada um dos conjuntos de bits de entrada a seguir:

a) 01
soma = 1
C_out = 0

b) 00
soma = 0
C_out = 0

c) 10
soma = 1
C_out = 0

d) 11
soma = 0
C_out = 1

3.Um somador-completo tem Cin = 1. Quais são a soma (Σ) e o carry de saída (Cout) quando A = 1 e B = 1?
soma = 1
C_out = 1

4.Use a tabela-verdade para determinar o resultado da adição dos números binários 1011 e 1010.
A = 1011
B = 1010

n1
A1 = 1
B1 = 0
Cin = 0
S = 1
Cout = 0

n2
A2 = 1
B2 = 1
Cin = 0
S = 0
Cout = 1

n3
A3 = 0
B3 = 0
Cin = 1
S = 1
Cout = 0

n4
A3 = 1
B3 = 1
Cin = 0
S = 0
Cout = 1

1011 + 1010 = 10101

5.Repita o processo para as entradas binárias 01 e 10.

![image](https://github.com/user-attachments/assets/b14a1231-2732-4aec-96a2-319c9906f2e7)

a = 01
b = 10

a0     b0
1 xor 0 = 1
a1     b1
0 xor 1 = 1

not 1 = 0
0 and 0 = 0

Valores diferentes

6.Quais são as saídas do comparador quando A3A2A1A0 = 1001 e B3B2B1B0 = 1010?

![image](https://github.com/user-attachments/assets/799b1b5b-2f71-432a-aa58-f22ed533171b)

a = 1001
b = 1010

a3 = b3
a2 = a2
a1 < b1

b é maior, ou seja 
A > B nível BAIXO
A = B nível BAIXO
A < B nível ALTO
