# jira-rules-trf5

# Regras de Automação Jira para Notificações no Google Chat

## Como Importar as Regras
1. **Acesse as Configurações Globais de Automação:** No Jira, clique no ícone de engrenagem no canto superior direito e selecione "Configurações do Sistema". Em seguida, na seção "Avançado", clique em "Regras de automação".
2. **Importar Regras:** No canto superior direito da tela de Automação Global, clique nos três pontos verticais (...) e selecione "Importar regras".
3. **Carregue o Arquivo JSON:** Clique em "Upload JSON" ou arraste e solte o arquivo `.json` da regra desejada na área indicada.
4. **Selecione as Regras e o Escopo:** Selecione as regras que você deseja importar e defina o escopo de projetos para cada uma.
5. **Importe os Proprietários das Regras (Opcional):** Marque a caixa "Importar proprietários de regras" para importar os proprietários do arquivo. Caso contrário, a pessoa que importou as regras será listada como proprietária.
6. **Ajuste os IDs de Conta (se aplicável):** Se estiver importando de um Jira Server/Data Center, você precisará alterar manualmente os IDs de conta dos proprietários das regras, pois eles são diferentes no Jira Cloud.
7. **Finalize a Importação:** Clique em "Vamos lá" para concluir o processo.

**Observações:**

* **Regras Desabilitadas:** Todas as regras importadas serão inicialmente desabilitadas. Você precisará ativá-las manualmente para que funcionem.
* **Nomes de Regras Duplicadas:** Se uma regra com o mesmo nome já existir, a regra importada terá o nome "Cópia de [nome da regra]".
* **Limite de Tamanho do Arquivo:** O arquivo JSON deve ter no máximo 5 MB. Se o arquivo for muito grande, exporte a regra em vários segmentos.

***Observação***: Certifique-se de que a integração com o Google Chat esteja configurada corretamente no Jira antes de importar as regras.

## Lista de Regras

+ [Tarefa com Alta Prioridade Editada](/tarefa-alta-prioridade-editada/README.md)
+ [Tarefa com Alta Prioridade Criada](/tarefa-alta-prioridade-criada/README.md)
+ [Tarefa Concluída/Resolvida](/tarefa-concluida-resolvida/README.md)
+ [Tarefa Bloqueada/Impedida](/tarefa-bloqueada-impedida/README.md)
+ [Tarefas (Iniciadas e não Concluidas) com mais de x dias sem atualizações](/tarefas-sem-atualizacao/README.md)
+ [Relatorio de atividades no fim do dia](/relatorio-fim-dia/README.md)
+ [Relatorio de atividades no começo do dia](/relatorio-inicio-dia/README.md)
+ [Sprint Finalizada](/sprint-finalizada/README.md)
+ [Sprint Iniciada](/sprint-iniciada/README.md)

***Lembre-se***: Adapte as regras de acordo com as necessidades específicas do seu projeto e fluxo de trabalho.