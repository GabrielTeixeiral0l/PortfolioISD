# Flip-Flops &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

- Blocos elementares sequenciais mais avançados que os latches.
- Alteram as saídas apenas em momentos específicos determinados por sinais de relógio (CLK).

### Tipos de Flip-Flops

1. **Flip-Flop D Edge-Triggered**
   - Entrada D amostrada no bordo ascendente ou descendente do CLK.
   - Estrutura Mestre-Escravo:
     - Mestre: Aberto quando CLK=0.
     - Escravo: Aberto quando CLK=1.

2. **Flip-Flop J-K**
   - Resolve o problema do estado inválido do S-R.
   - Quando J e K são ativados simultaneamente, as saídas alternam.
   - Característica: $Q^* = J \cdot \overline{Q} + \overline{K} \cdot Q$

3. **Flip-Flop T (Toggle)**
   - Alterna o estado em cada transição do CLK.
   - Frequência de saída é metade da frequência de entrada.

### Considerações de Funcionamento
- **Setup time** e **hold time**:
  - Entradas devem permanecer estáveis durante este intervalo para evitar valores imprevisíveis.
- Entradas assíncronas (PR, CLR):
  - Forçam estados independentes do CLK.
  - Utilizadas para inicialização e teste.

### Aplicações
- Armazenamento de estados em máquinas de estados finitas.
- Divisão de frequência e controlo lógico em sistemas digitais complexos.
