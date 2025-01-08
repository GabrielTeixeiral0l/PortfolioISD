# Latches &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

## O que são Latches
- Blocos elementares para circuitos sequenciais.
- Alteram as saídas em qualquer momento, independentemente de sinais de relógio.

### Tipos de Latches
1. **Latch S-R com portas NOR**
   - S (Set): Define a saída Q como 1.
   - R (Reset): Define a saída Q como 0.
   - Problema: Estado inválido ocorre quando S e R estão simultaneamente ativos (1).

2. **Latch S-R com portas NAND**
   - Entradas ativas em nível baixo.
   - Mantém o estado quando ambas entradas são desativadas (S_L=1, R_L=1).
   - Diferença: Quando ambas as entradas estão ativas, as saídas são 1 (e não 0).

3. **Latch S-R com Enable**
   - Inclui uma entrada de habilitação (C).
   - Reage às entradas S e R apenas quando C está ativa.

4. **Latch D**
   - Apenas uma entrada além de EN.
   - Saída Q segue a entrada D quando EN está ativo.
   - Recomendada para armazenamento de bits de informação.

### Funcionamento Geral
- Mantém o último valor enquanto EN está inativo.
- A entrada D deve permanecer fixa durante o intervalo definido por **setup time** e **hold time**.
