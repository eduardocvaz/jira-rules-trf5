## Notificação Jira - Sprint Iniciada

Esta automação envia uma notificação para o Google Chat sempre que uma nova sprint é iniciada no Jira. Fornece um resumo das informações relevantes da sprint, como nome, período, tempo restante, total de tarefas e tarefas priorizadas, ajudando a equipe a se preparar e se organizar para o novo ciclo de trabalho.

### Fluxo da Automação

1. **Gatilho:** A regra é acionada quando uma sprint é iniciada em um quadro Jira específico.
2. **Coleta de Dados:**
    * Coleta informações sobre o projeto e a sprint iniciada.
    * Busca todas as issues associadas à nova sprint.
    * Calcula o tempo restante da sprint, total de tarefas e lista as tarefas priorizadas.
    * Busca a mensagem de início da sprint de uma issue pré-definida.
3. **Criação do Relatório:** Gera um relatório com a mensagem de início da sprint, nome, período, tempo restante, total de tarefas, objetivo e lista de tarefas priorizadas.
4. **Envio de Notificação:** O relatório é enviado para um webhook configurado no Google Chat.

### Configuração

* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat.
* **Mensagem de Início da Sprint:** Crie uma issue no Jira com a mensagem desejada e especifique seu ID na variável "tarefaMensagem".

### Arquivos

* **[Sprint Iniciada → Notificar via webhook.json](./Sprint Iniciada → Notificar via webhook.json)**: Arquivo JSON com a regra pronta para importação no Jira Automation.

### Observações

* A automação utiliza JQL para consultar as issues relevantes.
* Personalize a mensagem de início da sprint para comunicar informações importantes à equipe.
* Essa automação promove a organização e o alinhamento da equipe no início de cada sprint, garantindo que todos estejam cientes das metas e prioridades.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!