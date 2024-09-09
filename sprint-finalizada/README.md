## Notificação Jira - Sprint Finalizada

Esta automação gera um relatório detalhado sobre o desempenho da sprint ao final dela e envia para o Google Chat, permitindo que a equipe avalie o progresso e identifique áreas de melhoria.

### Fluxo da Automação

1. **Gatilho:** A regra é acionada quando uma sprint é marcada como concluída em um quadro Jira específico.
2. **Coleta de Dados:**
    * Coleta informações sobre o projeto e a sprint finalizada.
    * Busca todas as issues associadas à sprint e as issues concluídas.
    * Calcula métricas como duração da sprint, total de tarefas, tarefas concluídas, etc.
3. **Criação de Relatórios:**
    * Gera um relatório geral da sprint com as métricas e o objetivo.
    * Opcionalmente, gera relatórios individuais para cada membro da equipe, detalhando suas tarefas concluídas.
4. **Envio de Notificações:** Os relatórios são enviados para um webhook configurado no Google Chat.

### Configuração

* **Webhook:** Certifique-se de que o webhook esteja configurado corretamente no Google Chat.
* **Relatórios Individuais:** Ative ou desative a opção "relatorioIndividual" conforme necessário.

### Notificação

![Imagem notificao!](/sprint-finalizada/images/img.png "Imagem da notificação no Google Chat")

### Observações

* A automação utiliza JQL para consultar as issues relevantes.
* As mensagens enviadas para o webhook são formatadas em JSON.
* Personalize a automação para se adequar às suas necessidades, como alterar o webhook, adicionar campos nos relatórios ou modificar os cálculos das métricas.
* Essa automação promove a transparência e a análise do desempenho da sprint, incentivando a melhoria contínua do processo.

---

**Dica:** Explore as outras regras de automação disponíveis neste repositório para otimizar ainda mais o seu fluxo de trabalho no Jira!