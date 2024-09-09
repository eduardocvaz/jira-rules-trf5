## Notificação Jira - Relatório de Atividades no Fim do Dia

Esta automação gera um relatório diário sobre o progresso da sprint em andamento, com foco nas tarefas concluídas naquele dia, e envia para um canal do Google Chat. Ajuda a equipe a acompanhar o andamento do projeto e a celebrar as conquistas diárias.

### Fluxo da Automação

1. **Gatilho:** A automação é executada diariamente em um horário agendado (atualmente às 18h, horário de Brasília).
2. **Coleta de Dados:**
    * Coleta o nome do projeto e a chave da issue com a mensagem de fim do dia.
    * Busca as issues concluídas naquele dia e associadas a sprints abertas.
    * Busca todas as issues associadas a sprints abertas.
    * Calcula a porcentagem de conclusão das tarefas do dia.
    * Busca a mensagem de fim do dia da issue especificada.
3. **Criação do Relatório:** Gera um relatório com a mensagem de fim do dia, nome da sprint, período, porcentagem de conclusão e tempo restante.
4. **Envio de Notificação:** O relatório é enviado para um webhook configurado no Google Chat.

### Configuração

* **Agendador:** Ajuste o horário de execução no agendador, se necessário.
* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat.
* **Mensagem de Fim do Dia:** Crie uma issue no Jira com a chave especificada e adicione a mensagem desejada na descrição.

### Arquivos

* **[Relatorio de atividades no fim do dia → Notificar via webhook.json](./Relatorio de atividades no fim do dia → Notificar via webhook.json)**: Arquivo JSON com a regra pronta para importação no Jira Automation.

### Observações

* A automação está atualmente desativada. Ative-a alterando o valor de "state" para `ENABLED`.
* Certifique-se de que as chaves das issues (mensagem de fim do dia) existam no seu projeto Jira.
* Essa automação promove a transparência e o reconhecimento do progresso diário, incentivando a equipe e mantendo o foco nos objetivos da sprint.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!