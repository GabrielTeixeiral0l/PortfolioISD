# Dispositivos de Memória &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

Um dispositivo de **memória binária** ou **digital** deve possibilitar:
- **escrita**: em que um valor binário é armazenado;
- **leitura**: em que um valor memorizado é lido para posterior utilização;

A sua implementação pode fazer-se, basicamente, de duas formas:
- Recorrendo a mecanismos analógicos
- Recorrendo a portas lógicas (com realimentação das saídas para as entradas)

Independentemente da forma pela qual é implementado, um dispositivo elementar de memória com capacidade para armazenar **um bit**, designa-se por **célula de memória**.

O elemento de memória mais simples de todos é o **bi-estável**.

## Bi-estável

O circuito de memória mais simples, é um circuito sem entradas e construído com um par de inversores interligados de modo a estabelecer um ciclo com feedback.

![Pasted image 20241222115313](https://github.com/user-attachments/assets/ff00a43b-cfdd-4406-870e-86537fbecf9d)

O nome deste circuito é **bi-estável** porque possui duas situações estáveis:
- Quando **Q está no nível ALTO**, o inversor inferior tem a saída no nível BAIXO, forçando deste modo o inversor superior a colocar a sua saída no nível ALTO (como se assumiu inicialmente).
 - Quando **Q está no nível BAIXO**, o inversor inferior tem a saída no nível ALTO, forçando deste modo o inversor superior a colocar a sua saída no nível BAIXO (como se assumiu inicialmente).
Pode usar-se uma única variável de estado (sinal Q) para definir o estado do circuito. Logo, há 2 estados possíveis: **Q=0 e Q=1**.

É impossível controlar um bi-estável, já que ele não tem entradas.
## Funcionamento de um bi-estável

O bi-estável está em equilíbrio nas posições assinaladas com “**stable**”.
Há um 3º ponto de equilíbrio, assinalado com “**metastable**”, que ocorre quando $V_{out1}$ e $V_{out2}$ não são nem 0 nem 1 lógico.

![Pasted image 20241222120201](https://github.com/user-attachments/assets/cf62088c-caa2-4e4d-9dcb-8e7c8d486813)

Se não houvesse ruído e o circuito atingisse o ponto meta-estável, poderia permanecer nele indefinidamente.
O ponto é meta-estável porque o ruído tenderá a levar o circuito para uma das posições estáveis.
