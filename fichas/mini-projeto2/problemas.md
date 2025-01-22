# Mini-Projeto 2 - Problemas &nbsp; [![Ir para README](https://img.shields.io/badge/Indice-Verde?style=for-the-badge)](../../README.md#indice)

Notas:
• São disponibilizados diversos problemas que necessitam de resolução.
• Cada aluno deverá escolher apenas um desses problemas. O trabalho é individual.
• Após a escolha, cada aluno deverá analisar e resolver o problema indicado da forma mais completa
possível.
• Deverá entregar a resolução do problema escolhido devidamente explicado e comentado.
• Para além de entregar a resolução do problema, deverá criar, preparar e apresentar o seu trabalho
na última aula do semestre.
• A avaliação do Mini-Projeto 2 inclui a resolução (60%) e a apresentação/defesa do trabalho (40%).

Problema 1
Dimensione um mecanismo automático de controlo das cancelas duma passagem de nível de acordo com
a figura abaixo. O sistema deve baixar as cancelas C1 e C2 quando passa um comboio e deve depois
levantar as cancelas para permitir a passagem de trânsito rodoviário em segurança. Os sensores S1 e S2
são sensores de presença, e estão normalmente a zero, mas assumem valor um quando passa um
comboio na sua frente. A distância de cada um dos sensores até à passagem de nível é muito maior do
que o comprimento do comboio.
Considere que podem passar comboios em ambas das direções mas o tempo entre duas passagens
sucessivas é bastante grande de forma que nunca existirão dois comboios em simultâneo no troço da
linha representado na figura.
Desenvolva o projeto do sistema descrito apresentando cada um dos passos:
a) O diagrama de estados;
b) A tabela de transição de estados;
c) Os estados redundantes;
d) A codificação de estados;
e) A tabela de transição com estados codificados;
f) O diagrama lógico do circuito;
g) Verifique se o sistema é autocorretor.

![image](https://github.com/user-attachments/assets/20a877f6-d773-4d4e-8a92-5aad079b6151)

Problema 2
Dimensione um mecanismo de controlo duma porta de abertura automática duma loja comercial de
acordo com a figura. Pretende-se um comportamento idêntico às portas que encontramos no quotidiano,
que abrem para deixar entrar ou sair clientes e voltam a fechar quando não há pessoas na proximidade.
O movimento da porta é realizado por um motor M cujo movimento é controlado apenas por um sinal
que define o sentido de rotação do motor. O motor tem sempre indicação para rodar no entanto pára
automaticamente quando a porta fica completamente aberta ou completamente fechada, pois em cada
um destes casos a porta oferece resistência ao movimento. Para determinar se a porta se encontra
completamente aberta existe um sensor A que fica ativo neste caso. A abertura e fecho da porta devem
obedecer ao seguinte critério:
• A porta deve manter-se fechada enquanto não forem detetadas pessoas através do sensor S;
• A porta inicia a abertura se o sensor S ficar ativo;
• Iniciada a abertura, esta só termina quando a porta se encontrar totalmente aberta (sensor A ficar
ativo) mesmo que durante a abertura o sensor S fique descativo;
• A porta depois de totalmente aberta inicia de imediato o fecho caso o sensor S esteja descativo,
caso contrário permanece aberta enquanto o sensor S se mantiver ativo;
• Durante o fecho, se o sensor S ficar ativo, então a porta reinicia imediatamente a abertura ainda
antes de fechar completamente de forma a ficar novamente aberta.
Desenvolva o projeto do sistema descrito apresentando cada um dos passos:
a) O diagrama de estados;
b) A tabela de transição de estados;
c) Os estados redundantes;
d) A codificação de estados;
e) A tabela de transição com estados codificados;
f) O diagrama lógico do circuito;
g) Verifique se o sistema é autocorretor

![image](https://github.com/user-attachments/assets/e1a165fd-1c65-4685-9316-f21bc7cbfeb8)


Problema 3
Dimensione um sistema para controlo de um túnel de lavagem automática de automóveis, como o
representado na figura.
O túnel de lavagem automática é composto por duas áreas de tratamento que um automóvel atravessa
sucessivamente. O sistema deteta a chegada de um automóvel através do laser (L) e ativa imediatamente
(coloca em funcionamento) a corrente de tração (C), que irá puxar o veículo ao longo de todo o túnel até
o processo de lavagem ser concluído. Na primeira zona de tratamento, são ativados/ligados os sistemas
de água com detergente (A) e as escovas de lavagem (E). Quando o veículo chega à segunda zona de
tratamento, esta presença é detetada pelo tapete (T). Ao detetar o veículo, o sistema desliga o
fornecimento de água com detergente e pára as escovas, colocando em funcionamento o sistema de
secagem com ventilação forçada (V). As ventoinhas de secagem (V) permanecem ativas (em
funcionamento) enquanto pelo menos uma das rodas do veículo estiver sobre o tapete (T). Quando o
veículo sai completamente do túnel, todos os dispositivos são desligados, e o sistema entra em estado de
espera por um novo automóvel. Considere que apenas um veículo entra no túnel de cada vez, isto é, só
entra um novo veículo no túnel após o anterior ter saído e concluído o processo.
Desenvolva o projeto do sistema descrito apresentando cada um dos passos:
a) O diagrama de estados;
b) A tabela de transição de estados;
c) Os estados redundantes;
d) A codificação de estados;
e) A tabela de transição com estados codificados;
f) O diagrama lógico do circuito;
g) Verifique se o sistema é autocorretor

![image](https://github.com/user-attachments/assets/dba9259b-e428-4318-8aec-395f0b0c4527)

Problema 4
Pretende-se um novo mecanismo de controlo de entrada de automóveis num determinado local de
acordo com a figura.
Neste novo sistema, o condutor no veículo deve introduzir uma moeda de 1 euro da caixa identificada por
Pagamento P na figura. Quando isso acontece, a Cancela C deve levantar e permanecer aberta,
possibilitando a passagem do veículo. Depois do veículo passar, a cancela deve fechar, aguardando a
chegada de outro veículo.
O Sensor Laser L tem como função obter informação da passagem do veículo na zona pela cancela.
Considere que só chega um novo veículo depois do anterior já ter entrado e que o controlo de saídas não
é da responsabilidade deste sistema.
Desenvolva o projeto do sistema descrito apresentando cada um dos passos:
a) O diagrama de estados;
b) A tabela de transição de estados;
c) Os estados redundantes;
d) A codificação de estados;
e) A tabela de transição com estados codificados;
f) O diagrama lógico do circuito;
g) Verifique se o sistema é autocorretor

![image](https://github.com/user-attachments/assets/94cb05a4-e933-4a7a-be6a-4311885f9cb6)
