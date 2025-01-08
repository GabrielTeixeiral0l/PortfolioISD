# Circuito Sequencial &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

Um **circuito sequencial** é um tipo de circuito digital no qual as saídas dependem não apenas das entradas atuais, mas também do **estado anterior** do circuito. 

Um circuito sequencial é constituído por um componente de memória e por um componente combinacional.

![image 1](https://github.com/user-attachments/assets/acfb5248-f406-49ef-9391-cdf7bd5c01b2)

O conjunto das saídas de todas as células de memória constitui o estado de um circuito sequencial.
O número de estados depende do número de Flip-Flops que o circuito contém, como cada Flip-Flop tem **dois** estados possíveis (**Q=0** ou **Q=1**), o número total de estados é $2^n$, sendo **n** o número de Flip-Flops do circuito.
Designam-se por **variáveis de estado**, as saídas da Unidade de Memória (uma variável por cada saída de um Flip-Flop).


No modelo geral de um **circuito sequencial**, define-se:
- **Descodificador de Saída** - é o circuito combinacional que gera as saídas externas do circuito sequencial;
- **Descodificador de Estado Seguinte** - é o circuito combinacional que gera as entradas para o bloco Unidade de Memória (estas são tais que, aplicadas aos Flip-Flops, resultarão numa combinação de variáveis de estado igual ao estado seguinte pretendido).
- **Análise de um circuito**: é o processo que permite obter uma descrição sobre o funcionamento do circuito, através do exame do seu diagrama lógico.
- **Síntese de um circuito**: é o processo que, a partir da descrição do funcionamento pretendido para o circuito, permite chegar ao diagrama lógico que traduz esse funcionamento.

O funcionamento de um circuito sequencial pode ser representado por:
- Diagrama de Estados
- Tabela de Transição
- Tabela de Excitação
