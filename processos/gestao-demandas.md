# Gestão de Projetos e Demandas

Este documento define a metodologia de organização de tarefas, projetos e chamados do Grupo de Desenvolvimento, utilizando o **Microsoft Planner** como ferramenta de gestão de fluxo e o **GLPI** para atendimento de chamados.

## 1. Estrutura de Fluxo no Microsoft Planner

Para garantir o controle entre o planejamento estratégico e a execução técnica, utilizamos uma estrutura dividida em três níveis de maturidade e temporalidade:

### Nível 1: Backlog de Demandas (Atemporal)
*   **O que é:** Repositório central de todas as tarefas, ideias e demandas futuras.
*   **Temporalidade:** Atemporal (contínuo).
*   **Objetivo:** Servir como base para triagem e priorização constante.
*   **Estrutura de Buckets (Origem):**
    *   **🎯 Radar Gestão:** Demandas estratégicas e prioridades da Direção.
    *   **👥 Usuários & Departamentos:** Solicitações via GLPI ou reuniões.
    *   **⚙️ Gestão TI:** Infraestrutura, segurança e governança.
    *   **🚀 Equipe (Inovação/Técnico):** Refatoração e débito técnico.

### Nível 2: Dashboard de Execução Global (Ciclo Anual)
*   **O que é:** Painel principal com as tarefas ativas do ano corrente (Ex: `Execução Global 2026`).
*   **Temporalidade:** Ciclo anual (Janeiro a Dezembro).
*   **Objetivo:** Centralizar as entregas do ano.
*   **Estrutura de Buckets (Sistemas/Ferramentas):**
    *   **📥 Triagem / Backlog:** Itens recém-promovidos do N1 aguardando início.
    *   **💻 Aplicações (Apps):** Sistemas próprios (Portal, Bolsas, etc).
    *   **📚 Bibliotecas & APIs (Libs):** Componentes e conectores.
    *   **🏢 Ecossistema TOTVS RM:** Customizações no ERP.
    *   **☁️ Plataformas & Terceiros:** Low-Code (Fluig, Power BI) e integrações externas.
    *   **📖 Documentação & Processos:** Manutenção do `team-docs` e cultura.

### Nível 3: Planners de Projetos (Ciclo do Projeto)
*   **O que é:** Painéis dedicados para grandes projetos ou implantações complexas.
*   **Temporalidade:** Vinculada ao cronograma do projeto (Início e Fim).
*   **Objetivo:** Detalhamento técnico e operacional específico.

---

## 2. Padronização e Identificação (Compartilhado)

Para manter a consistência entre todos os níveis (N1, N2 e N3), utilizamos os seguintes padrões:

### Tags (Categorização e Filtro)
As tags são idênticas em todos os Planners para permitir visão unificada:
*   **🎯 Radar Gestão:** Demandas estratégicas priorizadas pela Direção da Uniarp.
*   **🔴 Bug / Crítico:** Erros em produção que exigem ação imediata.
*   **🟡 Melhoria:** Evolução incremental de sistemas existentes.
*   **🟢 Novo Recurso:** Implementação de funcionalidades inéditas.
*   **🟠 Aguardando Revisão:** Bloqueio por definição funcional, aprovação ou revisão técnica/gerencial.
*   **🟣 Infraestrutura:** Dependência técnica de Rede/Servidores ou Atualizações de Plataforma.

### Nomenclatura
*   **Ano no Nome:** Painéis devem conter o ano (Ex: `Execução 2026`) para histórico.
*   **Rastreabilidade:** Cards no N2 que referenciam projetos N3 devem conter o link direto para o Planner do projeto.

---

## 3. Integração com GLPI (Chamados)

O GLPI é a porta de entrada para incidentes e solicitações (N2/N3):
1.  **Incidentes Rápidos:** Resolvidos diretamente no GLPI.
2.  **Bugs/Melhorias:** Geram card no Planner (N1 ou N2) referenciando o ticket do GLPI.
3.  **Fechamento:** O ticket só é encerrado após conclusão no Planner e validação.

---

## 4. Papéis e Responsabilidades por Nível

| Nível | Responsável | Atribuições Principais |
| :--- | :--- | :--- |
| **Estratégico** | **Gestor (Carlos)** | Arbitragem de prioridades macro e validação de resultados. |
| **N1: Backlog** | **Supervisor (Marcelo)** | Triagem de origens e priorização técnica inicial. |
| **N2: Execução** | **Supervisor / Analistas** | Gestão das tarefas ativas e acompanhamento de prazos. |
| **N3: Projetos** | **Analistas (Pontos Focais)** | Detalhamento técnico e atualização diária. |

---

## 5. Ganhos Estratégicos

*   **Foco Visual:** Separação clara entre o que é "origem" (N1) e o que é "entrega" (N2).
*   **Linguagem Comum:** Tags unificadas facilitam a transição de cards entre painéis.
*   **Foco na Conclusão:** Combate o acúmulo de cards parados através do ciclo anual.

---
*Este processo deve ser revisado anualmente durante a transição de ciclo dos Planners.*