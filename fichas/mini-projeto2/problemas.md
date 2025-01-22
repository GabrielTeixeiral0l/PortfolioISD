# Mini-Projeto 2 - Problemas &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)
# Notas

- São disponibilizados diversos problemas que necessitam de resolução.
- Cada aluno deverá escolher apenas um desses problemas. O trabalho é individual.
- Após a escolha, cada aluno deverá analisar e resolver o problema indicado da forma mais completa possível.
- Deverá entregar a resolução do problema escolhido devidamente explicado e comentado.
- Para além de entregar a resolução do problema, deverá criar, preparar e apresentar o seu trabalho na última aula do semestre.
- A avaliação do Mini-Projeto 2 inclui a resolução (60%) e a apresentação/defesa do trabalho (40%).

---

## Problema 1

Dimensione um mecanismo automático de controlo das cancelas de uma passagem de nível, de acordo com a figura abaixo. O sistema deve baixar as cancelas C1 e C2 quando passa um comboio e deve depois levantá-las para permitir a passagem de trânsito rodoviário em segurança.  

Os sensores S1 e S2 são sensores de presença, estando normalmente a zero, mas assumem o valor um quando passa um comboio na sua frente. A distância de cada um dos sensores até à passagem de nível é muito maior do que o comprimento do comboio.  

Considere que podem passar comboios em ambas as direções, mas o tempo entre duas passagens sucessivas é suficientemente grande para que nunca existam dois comboios em simultâneo no troço da linha representado na figura.  

Desenvolva o projeto do sistema descrito apresentando cada um dos passos:  
1. O diagrama de estados;  
2. A tabela de transição de estados;  
3. Os estados redundantes;  
4. A codificação de estados;  
5. A tabela de transição com estados codificados;  
6. O diagrama lógico do circuito;  
7. Verifique se o sistema é autocorretor.  

![Figura 1](https://github.com/user-attachments/assets/20a877f6-d773-4d4e-8a92-5aad079b6151)

---

## Problema 2

Dimensione um mecanismo de controlo de uma porta de abertura automática de uma loja comercial, de acordo com a figura. Pretende-se um comportamento idêntico às portas automáticas do quotidiano, que abrem para permitir a entrada ou saída de clientes e fecham quando não há pessoas na proximidade.  

O movimento da porta é realizado por um motor M, controlado apenas por um sinal que define o sentido de rotação. O motor pára automaticamente quando a porta atinge a posição completamente aberta ou fechada, devido à resistência oferecida. Para detetar se a porta está completamente aberta, existe um sensor A que fica ativo nesse caso.  

A abertura e fecho da porta devem obedecer ao seguinte critério:  
- A porta permanece fechada enquanto o sensor S não detetar pessoas;  
- A porta inicia a abertura se o sensor S ficar ativo;  
- Após iniciar a abertura, esta só termina quando a porta estiver completamente aberta (sensor A ativo), mesmo que o sensor S fique inativo;  
- Quando completamente aberta, a porta inicia o fecho se o sensor S estiver inativo; caso contrário, permanece aberta enquanto o sensor S estiver ativo;  
- Durante o fecho, se o sensor S ficar ativo, a porta reinicia imediatamente a abertura antes de fechar completamente.  

Desenvolva o projeto do sistema descrito apresentando cada um dos passos:  
1. O diagrama de estados;  
2. A tabela de transição de estados;  
3. Os estados redundantes;  
4. A codificação de estados;  
5. A tabela de transição com estados codificados;  
6. O diagrama lógico do circuito;  
7. Verifique se o sistema é autocorretor.  

![Figura 2](https://github.com/user-attachments/assets/e1a165fd-1c65-4685-9316-f21bc7cbfeb8)

---

## Problema 3

Dimensione um sistema de controlo para um túnel de lavagem automática de automóveis, como representado na figura.  

O túnel é composto por duas áreas de tratamento que um automóvel atravessa sucessivamente. O sistema deteta a chegada de um automóvel através do laser (L) e ativa a corrente de tração (C) para puxar o veículo ao longo do túnel até o processo ser concluído.  

- Na primeira zona, são ativados o sistema de água com detergente (A) e as escovas de lavagem (E).  
- Na segunda zona, detetada pelo tapete (T), desliga-se o fornecimento de água e as escovas, ativando-se o sistema de secagem com ventilação forçada (V).  
- As ventoinhas (V) permanecem ativas enquanto pelo menos uma roda do veículo estiver sobre o tapete (T).  
- Após o veículo sair completamente, o sistema desliga todos os dispositivos e aguarda a chegada de outro automóvel.  

Desenvolva o projeto do sistema descrito apresentando cada um dos passos:  
1. O diagrama de estados;  
2. A tabela de transição de estados;  
3. Os estados redundantes;  
4. A codificação de estados;  
5. A tabela de transição com estados codificados;  
6. O diagrama lógico do circuito;  
7. Verifique se o sistema é autocorretor.  

![Figura 3](https://github.com/user-attachments/assets/dba9259b-e428-4318-8aec-395f0b0c4527)

---

## Problema 4

Dimensione um mecanismo de controlo de entrada de automóveis num local específico, de acordo com a figura.  

Neste sistema, o condutor deve introduzir uma moeda de 1 euro na caixa de pagamento (P). Quando isso ocorre, a cancela (C) levanta e permanece aberta, permitindo a passagem do veículo. Após o veículo passar, a cancela deve fechar, aguardando o próximo veículo.  

O Sensor Laser (L) deteta a passagem do veículo pela zona da cancela. Considere que um novo veículo só chega após o anterior ter entrado e que o controlo de saídas não é responsabilidade deste sistema.  

Desenvolva o projeto do sistema descrito apresentando cada um dos passos:  
1. O diagrama de estados;  
2. A tabela de transição de estados;  
3. Os estados redundantes;  
4. A codificação de estados;  
5. A tabela de transição com estados codificados;  
6. O diagrama lógico do circuito;  
7. Verifique se o sistema é autocorretor.  

![Figura 4](https://github.com/user-attachments/assets/94cb05a4-e933-4a7a-be6a-4311885f9cb6)
