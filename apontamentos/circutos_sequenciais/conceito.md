# Circuito Sequencial &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../README.md#indice)


Os circuitos sequenciais são sistemas digitais em que as saídas dependem não apenas das entradas atuais, mas também da sequência de valores anteriores das entradas. Isso significa que possuem memória, permitindo que o estado atual seja influenciado por valores passados.

## Características Principais

- **Dependência do Estado Atual:** O estado do circuito guarda informações sobre o passado, sendo necessário para prever o próximo estado.
- **Memória:** Os estados são representados por variáveis binárias internas ao circuito.
- **Máquinas de Estados Finitos:** Podem ser modelados como máquinas com um número limitado de estados possíveis.

### Estado e Transições

- O estado de um circuito sequencial é determinado pelas variáveis de estado.
- As mudanças de estado são reguladas por um sinal de relógio (clock).
  - Sinal ativo em bordos ascendentes ou descendentes, ou em níveis alto/baixo.
- Período do relógio (T) e frequência (f) têm relação inversa: \( f = \frac{1}{T} \).

### Exemplos

- Controle remoto de TV: Permite alternar entre canais com botões que dependem do estado atual e histórico.
