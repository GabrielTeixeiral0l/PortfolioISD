# Circuitos Integrados &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../README.md#indice)

Um **circuito integrado (CI)** é uma pequena área de material semicondutor (geralmente silício) onde são construídos componentes eletrónicos, como:
- Transístores
- Díodos
- Resistências
- Condensadores  

Estes componentes trabalham juntos para implementar uma função específica.

## Estrutura do CI
- O **chip** (ou **pastilha**) é a parte funcional do CI.  
- A maior parte do tamanho do CI é ocupada pelo invólucro exterior e pelas ligações aos terminais externos (**pinos**).

## Classificação dos CIs

### 1. Por **Famílias Lógicas**
Os **circuitos integrados digitais** são agrupados em famílias, dependendo da tecnologia de fabrico:
#### Famílias Bipolares:
- **RTL**: Resistor Transistor Logic  
- **DTL**: Diode Transistor Logic  
- **TTL**: Transistor Transistor Logic  
- **HTL**: High Threshold Logic  
- **ECL**: Emitter Coupled Logic  
- **I2L**: Integrated-Injection Logic  

#### Famílias MOS:
- **CMOS**: Complementary MOS (pares NMOS/PMOS)  
- **NMOS**: Apenas transístores MOS-FET canal N  
- **PMOS**: Apenas transístores MOS-FET canal P  

### 2. Por **Aplicação**
- **Lineares ou Analógicos**:
  - **Lineares**: Geram sinais contínuos em função das entradas.
  - **Analógicos**: Amplificam sinais (ex.: amplificadores operacionais).  
- **Digitais**:
  - Trabalham com estados lógicos (geralmente **0** e **1**).

### 3. Por **Densidade de Integração**
Os CIs podem ser classificados de acordo com a quantidade de componentes que integram. Exemplos incluem:

|                Categoria                 | Nº de Portas Lógicas por CI |
| :--------------------------------------: | :-------------------------- |
|    **SSI (Small-Scale Integration)**     | <12                         |
|    **MSI (Medium-Scale Integration)**    | 12 a 99                     |
|    **LSI (Large-Scale Integration)**     | 100 a 9 999                 |
| **VLSI (Very Large-Scale Integration)**  | 10 000 a 99 999             |
| **ULSI (Ultra Large-Scale Integration)** | 100 000 a 999 999           |
|     **GSI (Giga-Scale Integration)**     | >=1 000 000                 |


## Transístores: A Base dos CIs
- Nos sistemas digitais, o **transístor** funciona como um interruptor que controla o fluxo de corrente.
- São essenciais para todas as funções realizadas pelos CIs.

## Planta de Montagem

O projeto de Sistemas Digitais envolve uma fase inicial de dimensionamento de diagrama lógico com base num conjunto de procedimentos de projeto. 
- Considere-se o exemplo da implementação da seguinte função:

![Pasted image 20241122163617](https://github.com/user-attachments/assets/00022a4f-68a7-4cdd-a463-8209f8757992)

![Pasted image 20241122164539](https://github.com/user-attachments/assets/f713fde8-5ca5-41f1-9c15-617abae5da7a)

Na Planta de Montagem são representados: 
- Os circuitos integrados necessários;
- As ligações previstas no diagrama lógico;
- As ligações dos pinos de alimentação a 5 Volts;
- Ligação dos pinos de massa a 0 Volts;

![Pasted image 20241122164639](https://github.com/user-attachments/assets/0fa2d5ee-c424-4576-b85d-dabf53e95fea)

