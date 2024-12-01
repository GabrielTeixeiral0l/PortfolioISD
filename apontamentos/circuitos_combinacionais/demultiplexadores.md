# Circuitos Combinacionais - Demultiplexadores &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

Um **Demultiplexador (DEMUX)** realiza a operação inversa de um **Multiplexador (MUX)**.
- Recebe dados digitais de uma **única entrada** e distribui-os para **múltiplas saídas** com base no estado das **linhas de seleção de dados**.
- Também é conhecido como **distribuidor de dados**.

## Funcionamento
1. **Entrada de dados única:** Conectada a todas as portas lógicas AND.
2. **Linhas de seleção de dados:** Ativam uma porta lógica de cada vez, permitindo que os dados sejam transmitidos para a saída correspondente.

**Exemplo:**  
Para um DEMUX de 1 para 4:
- Entrada de dados: $D_\text{in}$
- Linhas de seleção: $S_0, S_1$
- Saídas: $D_0, D_1, D_2, D_3$

| $S_1$ | $S_0$ | **Saída Ativada** |
|-------|-------|-------------------|
| 0     | 0     | $D_0$            |
| 0     | 1     | $D_1$            |
| 1     | 0     | $D_2$            |
| 1     | 1     | $D_3$            |

---

### Aplicações
Os DEMUX são amplamente utilizados em:
- **Distribuição de sinais de clock:** Envia pulsos de sincronização para múltiplos destinos.
- **Transmissão de dados síncronos em série:** Em sistemas de comunicação, onde:
  - Um **MUX** é usado no emissor.
  - Um **DEMUX** é usado no recetor para separar os dados.

---

### Circuito DEMUX 1 para 4

1. **Componentes principais:**
   - Portas AND ligadas à entrada de dados.
   - Linhas de seleção que controlam a ativação das portas.

2. **Comportamento:**
   - Apenas uma porta AND é ativada de cada vez, dependendo da combinação das linhas de seleção.
   - Os dados de entrada são transmitidos para a saída correspondente.

![[Pasted image 20241201113446.png]]

---

### Exemplo Prático
#### Dados fornecidos:
- Entrada de dados: Onda quadrada.
- Linhas de seleção: $S_0$ e $S_1$ seguem uma sequência binária repetitiva $00, 01, 10, 11$.
#### Saídas:
- A cada ciclo, os dados de entrada são enviados para uma saída diferente ($D_0$ a $D_3$) com base no estado das linhas de seleção.

![[Pasted image 20241201113630.png]]

## CI Demultiplexador 74HC154

- Possui 16 saídas e 4 linhas de seleção ($2^4 = 16$).
- Linhas de seleção determinam qual saída está ativa.
- Em modo DEMUX:
  - Uma das entradas de seleção pode ser usada como linha de entrada de dados.
  - Todas as outras linhas devem ser configuradas adequadamente para habilitar o circuito.

**Exemplo de Configuração:**  
- Código binário nas linhas de seleção: $1010$  
- Entrada de dados: Nível BAIXO ($0$)  
**Resultado:** Apenas a linha de saída correspondente ao código $1010$ será ativada.
![[Pasted image 20241201113716.png]]
