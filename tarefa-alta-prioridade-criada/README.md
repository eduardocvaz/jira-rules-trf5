## Notificação Jira - Tarefa com Alta Prioridade Criada

Esta regra de automação envia uma notificação urgente para o Google Chat sempre que uma nova tarefa com alta prioridade é criada no Jira. Garante que a equipe seja imediatamente informada sobre tarefas críticas, permitindo uma ação rápida e priorização adequada.

### Fluxo da Automação

1. **Gatilho:** A regra é acionada quando uma nova issue é criada.
2. **Condições:**
    * A prioridade da issue deve ser "Alta" ou superior.
    * A issue deve pertencer a uma sprint que já foi iniciada.
3. **Coleta de Dados:** A regra coleta informações relevantes sobre a nova issue, como tipo, projeto, descrição, criador, status, etc.
4. **Envio de Notificação:** Uma mensagem detalhada é enviada para um webhook configurado no Google Chat, incluindo um alerta sobre a nova tarefa e seus detalhes.

### Configuração

* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat para receber as notificações.
* **Prioridade Mínima:** Ajuste a configuração "Prioridade Mínima" se desejar incluir outras prioridades além de "Alta".

### Notificação

![Imagem notificao!](/tarefa-alta-prioridade-criada/images/img.png "Imagem da notificação no Google Chat")


### Observações

* Personalize a mensagem de notificação no Google Chat para atender às necessidades da sua equipe.
* Essa automação garante que tarefas importantes sejam prontamente comunicadas à equipe, evitando atrasos e perda de foco.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!