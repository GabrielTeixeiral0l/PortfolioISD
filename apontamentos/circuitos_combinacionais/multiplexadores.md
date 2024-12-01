# Multiplexadores &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

- Possuem **múltiplas entradas** e **uma única saída**.
- Permitem selecionar uma entrada para ser reproduzida na saída.
- A seleção é feita através de um **código binário** aplicado às linhas de seleção.
## Aplicações:
- Seleção de dados
- Conversão paralelo-série
- Implementação de funções lógicas


## Diagrama Lógico de um MUX 4-bit:
- Utiliza duas linhas de seleção para determinar qual das 4 entradas será direcionada à saída.

**Exemplo:**  
Dados: $D0 = 0, D1 = 0, D2 = 1, D3 = 0$
Seletores: $S0 = 1, S1 = 0$  
Saída: $0$

![Pasted image 20241201104618](https://github.com/user-attachments/assets/488b3c11-afcb-4d97-b8c8-f2aeb46c3649)

![Pasted image 20241201104828](https://github.com/user-attachments/assets/e0db6f52-6495-4b01-858e-e30f7e9feab5)

![Pasted image 20241201104908](https://github.com/user-attachments/assets/d4ee740c-4956-473a-8850-aeaeac761b5f)


## Multiplexadores CI 74HC157

### Características:
- Contém **quatro multiplexadores de 2 entradas separados**.
- Linha de habilitação:
  - **Nível BAIXO**: dados passam para a saída.
  - **Nível ALTO**: multiplexadores desabilitados.

![Pasted image 20241201105318](https://github.com/user-attachments/assets/f80e05b5-5fcb-4b98-a0d4-5adb5004dc42)

### Tabela Verdade:
- **Strobe = H**: circuito desativado.
- **Strobe = L**: circuito ativado.
- Seletores determinam qual entrada é transmitida à saída $Y$.
- As letras $X$ presentes nas entradas da tabela de verdade, significam: “qualquer que seja o valor lógico da entrada...” 
- **Select** seleciona uma das entradas $A$ ou $B$ - esta seleção é comum aos 4 Multiplexadores
- A saída $Y$ reproduz a entrada selecionada

![Pasted image 20241201110108](https://github.com/user-attachments/assets/2b36eadb-79e7-4570-ac7e-a5a78335e4f5)


---

## Multiplexador de 8 Entradas (CI 74LS151)

### Características:
- 8 entradas de dados.
- 3 linhas de seleção para endereçar qualquer uma das 8 entradas ($2^3 = 8$).
- Disponibiliza saída de dados e o seu complemento.

![Pasted image 20241201110659](https://github.com/user-attachments/assets/a8db1c03-a4bd-4099-9c20-6f438ef20825)

### Exemplo:
- Multiplexar 16 linhas de dados numa única saída:
  - Usar dois **CIs 74LS151**.
  - A entrada de habilitação atua como o bit mais significativo.

![Pasted image 20241201110935](https://github.com/user-attachments/assets/989845c2-cba0-47d3-81af-2ee48d1600fd)


## Multiplexador para Display de 7 Segmentos

### Visão Geral
- Este circuito utiliza um multiplexador para alternar entre **dois dígitos BCD**:
  - **Dígito A:** $A_3A_2A_1A_0$
  - **Dígito B:** $B_3B_2B_1B_0$
- A alternância é controlada por uma **onda quadrada** aplicada à linha de seleção de dados.

### Funcionamento
1. **Quando a linha de seleção de dados está em nível BAIXO (0):**
   - Os bits do **dígito A** são passados para o **decodificador BCD para 7 segmentos** (**CI 74LS47**).
   - O **decodificador 74LS139** ativa a saída 0, ligando o display do dígito A ao GND.
   - **Resultado:** O dígito A está visível enquanto o dígito B está desligado.

2. **Quando a linha de seleção de dados está em nível ALTO (1):**
   - Os bits do **dígito B** são passados para o **decodificador BCD para 7 segmentos**.
   - O **decodificador 74LS139** ativa a saída 1, ligando o display do dígito B.
   - **Resultado:** O dígito B está visível enquanto o dígito A está desligado.

### Frequência de Alternância
- O ciclo de alternância entre os dois dígitos repete-se na frequência da onda quadrada.
- **Nota importante:** A frequência deve ser suficientemente alta ($\geq 30\, \text{Hz}$) para evitar cintilação visível nos displays.

---

### Exemplo de Aplicação
1. Dois números BCD diferentes são aplicados às entradas do multiplexador:
   - Dígito A: $1001$ (9)
   - Dígito B: $0110$ (6)
2. Uma onda quadrada com frequência de $60\, \text{Hz}$ alterna entre os dígitos.
3. O resultado visível no display é uma alternância rápida entre 9 e 6, aparentando que ambos os números estão ativos simultaneamente.


![Pasted image 20241201113446](https://github.com/user-attachments/assets/11f916f5-9e16-4c6b-b3a0-78a8bc395798)

