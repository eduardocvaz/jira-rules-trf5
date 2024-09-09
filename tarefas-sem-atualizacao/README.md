## Notificação Jira - Tarefas (Iniciadas e não Concluídas) com mais de x dias sem atualizações

Esta automação identifica tarefas em andamento que estão há um determinado número de dias sem atualizações e notifica a equipe sobre elas por meio do Google Chat. Ajuda a manter o foco nas tarefas que precisam de atenção e a identificar possíveis bloqueios ou atrasos no projeto.

### Fluxo da Automação

1. **Gatilho:** A automação é executada diariamente em um horário agendado (atualmente às 8h30, horário de Brasília).
2. **Coleta de Dados:**
    * Coleta o nome do projeto e o número de dias de atraso para considerar uma tarefa como atrasada.
    * Busca as issues que pertencem ao projeto, não estão concluídas ou novas, estão em sprints abertas e não foram atualizadas nos últimos X dias.
3. **Condição:** Verifica se existem issues atrasadas. Se não houver, a automação não prossegue.
4. **Envio de Notificação Inicial:** Se houver issues atrasadas, uma mensagem inicial é enviada para o Google Chat informando sobre a existência de tarefas atrasadas.
5. **Agrupamento por Status:** Agrupa as issues atrasadas por status.
6. **Envio de Notificações Detalhada por Status:** Para cada status, envia uma mensagem para o Google Chat com a lista de issues atrasadas nesse status, incluindo chave, resumo e responsável.

### Configuração

* **Agendador:** Ajuste o horário de execução no agendador, se necessário.
* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat.
* **Número de Dias de Atraso:** Ajuste o valor da variável "diasAtraso" conforme necessário.

### Notificação

![Imagem notificao!](/tarefas-sem-atualizacao/images/img.png "Imagem da notificação no Google Chat")

### Observações

* Personalize a mensagem de notificação no Google Chat para incluir mais informações sobre as issues, como prioridade ou data de vencimento.
* Essa automação promove a proatividade na gestão de tarefas, incentivando a equipe a manter as issues atualizadas e a resolver possíveis bloqueios.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!