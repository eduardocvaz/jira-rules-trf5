## Notificação Jira - Tarefa com Alta Prioridade Editada

Esta regra de automação envia uma notificação urgente para o Google Chat quando a prioridade de uma tarefa é alterada para "Alta" ou superior. Garante que a equipe seja alertada sobre mudanças críticas nas prioridades, permitindo uma resposta rápida e um ajuste de foco.

### Fluxo da Automação

1. **Gatilho:** A regra é acionada quando o campo de prioridade de uma issue é alterado.
2. **Condições:**
    * A nova prioridade da issue deve ser "Alta" ou superior.
    * A alteração no campo de prioridade deve ser para um nível mais alto.
    * A issue deve pertencer a uma sprint que já foi iniciada.
3. **Coleta de Dados:** A regra coleta informações relevantes sobre a issue editada, como tipo, projeto, descrição, criador, status, etc.
4. **Envio de Notificação:** Uma mensagem detalhada é enviada para um webhook configurado no Google Chat, incluindo um alerta sobre a mudança de prioridade e os detalhes da tarefa.

### Configuração

* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat para receber as notificações.
* **Prioridade Mínima:** Ajuste a configuração "Prioridade Mínima" se desejar incluir outras prioridades além de "Alta".

### Arquivos

* **[Tarefa com Alta Prioridade Editada → Notificar via webhook.json](./Tarefa com Alta Prioridade Editada → Notificar via webhook.json)**: Arquivo JSON com a regra pronta para importação no Jira Automation.

### Observações

* Personalize a mensagem de notificação no Google Chat para atender às necessidades da sua equipe.
* Essa automação promove a comunicação eficiente e a colaboração, garantindo que todos estejam cientes das mudanças importantes nas prioridades das tarefas.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para aprimorar ainda mais o seu fluxo de trabalho no Jira!