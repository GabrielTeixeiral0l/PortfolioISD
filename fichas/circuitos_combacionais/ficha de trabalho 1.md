# Ficha de trabalho 1 - Circuitos Combacionais &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

1. Identifique cada dispositivo a seguir: 74LS157 e 74LS151

O 74LS157 é um circuito integrado composto 4 seletores de dados de 2 entradas
O 74LS151 é um circuito integrado composto 1 seletor de dados de 8 entradas

3. Um CI 74LS151 tem alternadamente níveis BAIXO e ALTO nas suas entradas de dados começando por D0. As linhas de seleção de dados são recebem uma sequência de contagem binária (000, 001, 010 e assim por diante) numa frequência de 1 kHz. A entrada de habilitação é nível BAIXO. Descreva a forma de onda na saída de dados.


| S2  | S1  | S0  | ENTRADA SELECIONADA | SAÍDA |
| --- | --- | --- | :-----------------: | ----- |
| 0   | 0   | 0   |         D0          | 0     |
| 0   | 0   | 1   |         D1          | 1     |
| 0   | 1   | 0   |         D2          | 0     |
| 0   | 1   | 1   |         D3          | 1     |
| 1   | 0   | 0   |         D4          | 0     |
| 1   | 0   | 1   |         D5          | 1     |
| 1   | 1   | 0   |         D6          | 0     |
| 1   | 1   | 1   |         D7          | 1     |

A onda de saída vai alternando entre baixo e cima, conforme a sequencia das entradas de seleção.

3. Descreva resumidamente a finalidade de cada um dos seguintes dispositivos vistos na Figura do slide 24: 74LS157, 74LS47 e 74LS139
![Pasted image 20241129154351](https://github.com/user-attachments/assets/8dc6a2f3-65f1-4d73-a93e-02da8c661319)

74LS157 -  multiplexa os dois códigos BCD para o decodificador de 7 segmentos
74LS47 -  descodifica o numero BCD para energizar o display
74LS139 -  habilita alternadamente os displays.

4. Em geral, como um decodificador pode ser usado como um demultiplexador?
Um decodificador pode ser usado como demultiplexador porque ambos direcionam um sinal de entrada para uma das várias saídas, com base nas entradas de seleção. O decodificador escolhe qual saída ativar, e essa função é a mesma de um demultiplexador, que direciona o sinal de entrada para uma saída específica usando as mesmas linhas de seleção.

5. O CI demultiplexador 74HC154 mostrado na Figura do slide anterior tem um código binário de 1010 nas linhas de seleção de dados e a linha de entrada de dados é nível BAIXO. Quais são os estados das linhas de saída?

![Pasted image 20241129165418](https://github.com/user-attachments/assets/db892d63-6d4b-44d0-bede-b693bb1987fb)

A porta d10 vai estar em nível baixo e as outras em nível alto.

7. Em geral, um multiplexador tem 
(a) uma entrada de dados, diversas saídas de dados e entradas de seleção 
(b) uma entrada de dados, uma saída de dados e uma entrada de seleção 
(c) diversas entradas de dados, diversas saídas de dados e entradas de seleção 
->**(d) diversas entradas de dados, uma saída de dados e entradas de seleção**<-

8. Identifique do que se trata o seguinte circuito:

![image](https://github.com/user-attachments/assets/efbca069-dd37-4c04-af05-07a3d20e54c3)

a. MUX 4:1 
->**b. DEMUX 1:8**<-
c. Codificador Decimal para Binário 
d. Decodificador BCD para Display de 7 segmentos 
e. Decodificador Binário para Decimal
f. MUX 8:1 
g. DEMUX 1:4 

10. Analisando o circuito do exercício anterior, qual é o bit de seleção menos significativo (LSB)?
->**a. S0**<-
b. S1 
c. S2 
d. Z 
e. I0
f. I7 
g. E7 


11. Explique o que o circuito está a realizar:

![Pasted image 20241129172031](https://github.com/user-attachments/assets/2f0995cd-e328-44d7-84bc-1d862d84de81)

O circuito faz uma multiplexação de 16 entradas ($D0$ a $D15$) para uma saída. Para isso utiliza 2 multiplexadores de 8:1 e um de 2:1.
