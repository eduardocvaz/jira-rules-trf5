## Notificação Jira - Relatório de Atividades no Começo do Dia

Esta automação gera um relatório diário sobre o progresso da sprint em andamento e envia para um canal do Google Chat, motivando a equipe no início do dia com informações sobre o andamento do projeto.

### Fluxo da Automação

1. **Gatilho:** A automação é executada diariamente em um horário agendado (atualmente às 8h, horário de Brasília).
2. **Coleta de Dados:**
    * Coleta o nome do projeto e a chave da issue com a mensagem de bom dia.
    * Busca as issues concluídas e associadas a sprints abertas.
    * Busca todas as issues associadas a sprints abertas.
    * Calcula a porcentagem de conclusão da sprint.
    * Busca a mensagem de bom dia da issue especificada.
3. **Criação do Relatório:** Gera um relatório com a mensagem de bom dia, nome da sprint, período, tempo restante e porcentagem de conclusão.
4. **Envio de Notificação:** O relatório é enviado para um webhook configurado no Google Chat.

### Configuração

* **Agendador:** Ajuste o horário de execução no agendador, se necessário.
* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat.
* **Mensagem de Bom Dia:** Crie uma issue no Jira com a chave especificada e adicione a mensagem desejada na descrição.

### Arquivos

* **[Relatorio de atividades no começo do dia → Notificar via webhook.json](./Relatorio de atividades no começo do dia → Notificar via webhook.json)**: Arquivo JSON com a regra pronta para importação no Jira Automation.

### Observações

* A automação está atualmente desativada. Ative-a alterando o valor de "state" para `ENABLED`.
* Certifique-se de que as chaves das issues (mensagem de bom dia) existam no seu projeto Jira.
* Essa automação promove a transparência e o acompanhamento do progresso da sprint, incentivando a equipe e fornecendo uma visão geral no início de cada dia.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!