## Notificação Jira - Tarefa Bloqueada/Impedida

Esta automação envia uma notificação para o Google Chat quando uma tarefa é movida para o status "Bloqueada/Impedida" em uma sprint ativa. Alerta a equipe sobre o impedimento e solicita uma resolução rápida, promovendo a colaboração e a remoção de obstáculos.

### Fluxo da Automação

1. **Gatilho:** A regra é acionada quando uma issue sofre uma transição e o status de destino é "Bloqueada/Impedida".
2. **Condição:**
    * A issue deve pertencer a uma sprint que já foi iniciada.
3. **Coleta de Dados:** A regra coleta informações relevantes sobre a issue bloqueada, como tipo, projeto, descrição, criador, status, etc.
4. **Envio de Notificação:** Uma mensagem detalhada é enviada para um webhook configurado no Google Chat, incluindo um alerta sobre o bloqueio e os detalhes da tarefa.

### Configuração

* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat para receber as notificações.
* **Status "Bloqueada/Impedida":** Verifique se o ID do status "Bloqueada/Impedida" no seu Jira corresponde a 10014. Se for diferente, ajuste a configuração do gatilho.

### Arquivos

* **[Tarefa Bloqueada/Impedida → Notificar via webhook.json](./Tarefa Bloqueada/Impedida → Notificar via webhook.json)**: Arquivo JSON com a regra pronta para importação no Jira Automation.

### Observações

* Personalize a mensagem de notificação no Google Chat para atender às necessidades da sua equipe.
* Essa automação promove a visibilidade de problemas e incentiva a colaboração para a resolução rápida de bloqueios, mantendo o projeto em andamento.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!