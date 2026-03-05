# Gestão de Projetos e Demandas

Este documento define a metodologia de organização de tarefas, projetos e chamados do Grupo de Desenvolvimento, utilizando o **Microsoft Planner** como ferramenta de gestão de fluxo e o **GLPI** para atendimento de chamados.

## 1. Estrutura de Fluxo no Microsoft Planner

Para garantir o controle entre o planejamento estratégico e a execução técnica, utilizamos uma estrutura dividida em três níveis de maturidade e temporalidade:

### Nível 1: Backlog de Demandas (Atemporal)
*   **O que é:** Repositório central de todas as tarefas, ideias e demandas futuras (extraídas do planejamento em Excel e novas solicitações).
*   **Temporalidade:** Atemporal (contínuo).
*   **Objetivo:** Servir como base para triagem e priorização constante. É o "estacionamento" de ideias que ainda não entraram em execução.

### Nível 2: Dashboard de Execução Global (Ciclo Anual)
*   **O que é:** Painel principal com as tarefas ativas do ano corrente (Ex: `Execução Global 2026`).
*   **Temporalidade:** Ciclo anual (Janeiro a Dezembro).
*   **Objetivo:** Centralizar o que está sendo entregue no ano. Ao final do ciclo, o painel é arquivado, gerando o relatório consolidado de entregas daquele ano.

### Nível 3: Planners de Projetos (Ciclo do Projeto)
*   **O que é:** Painéis dedicados para grandes projetos ou implantações complexas (Ex: `PRJ-2026 | Implantação Valorizza`).
*   **Temporalidade:** Vinculada ao cronograma do projeto (Início e Fim definidos).
*   **Objetivo:** Detalhamento técnico e operacional de entregas específicas. Uma vez concluído o projeto, o Planner é arquivado.

---

## 2. Padronização e Visibilidade

*   **Nomenclatura:** Todos os projetos e painéis devem conter o ano no nome (Ex: `Execução 2026`) para facilitar a busca histórica e evitar confusão com anos anteriores.
*   **Rastreabilidade:** Cards no **Painel Global** que referenciam projetos específicos devem conter o link para o respectivo **Planner de Projeto**, mantendo a conexão entre o macro e o micro.

---

## 3. Integração com GLPI (Chamados)

O GLPI continua sendo a ferramenta oficial para incidentes e solicitações de usuários (N2/N3). O fluxo de integração segue estas premissas:

1.  **Incidentes Rápidos:** São resolvidos diretamente no ticket do GLPI.
2.  **Bugs de Código / Melhorias:** Geram um card no **Backlog** ou **Execução Global** do Planner, com o número do ticket do GLPI referenciado para rastreabilidade.
3.  **Fechamento:** O ticket no GLPI só é encerrado após a conclusão da tarefa no Planner e validação com o solicitante.

---

## 4. Ganhos Estratégicos

*   **Limpeza Visual:** Foco total no que tem prazo, mantendo o que não é prioridade "escondido" no Backlog.
*   **Mensuração de Resultados:** Facilita a prestação de contas anual e o planejamento do ciclo seguinte.
*   **Foco na Conclusão:** Combate o acúmulo de cards parados ao forçar o encerramento de painéis temporais.

---
*Este processo deve ser revisado anualmente durante a transição de ciclo dos Planners.*
