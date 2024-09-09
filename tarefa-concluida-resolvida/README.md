## Notificação Jira - Tarefa Concluída/Resolvida

Esta automação envia uma notificação para o Google Chat sempre que uma tarefa é concluída ou resolvida no Jira. Mantém a equipe informada sobre o progresso do projeto e permite que os membros acompanhem as tarefas que foram finalizadas.

### Fluxo da Automação

1. **Gatilho:** A regra é acionada quando o status de uma issue é alterado para "Concluído" ou "Resolvido".
2. **Coleta de Dados:** A regra coleta informações relevantes sobre a issue concluída/resolvida, como tipo, projeto, descrição, responsável, etc.
3. **Envio de Notificação:** Uma mensagem informativa é enviada para um webhook configurado no Google Chat, incluindo detalhes sobre a tarefa finalizada.

### Configuração

* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat para receber as notificações.

### Arquivos

* **[Tarefa Concluída/Resolvida → Notificar via webhook.json](./Tarefa Concluída/Resolvida → Notificar via webhook.json)**: Arquivo JSON com a regra pronta para importação no Jira Automation.

### Observações

* Personalize a mensagem de notificação no Google Chat para atender às necessidades da sua equipe.
* Essa automação promove a transparência e o acompanhamento do progresso do projeto, mantendo todos informados sobre as tarefas concluídas.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!

**Observação:** A descrição original fornecida para esta regra parecia estar relacionada à criação de tarefas com alta prioridade. Adaptei a descrição para refletir o título "Tarefa Concluída/Resolvida" e o gatilho mencionado. Se a intenção era diferente, por favor, forneça mais detalhes para que eu possa ajustar a descrição adequadamente.