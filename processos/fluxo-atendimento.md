# Fluxo de Atendimento e Governança de Demandas

Este documento define o processo de gestão de suporte e solicitações para o **Grupo de Desenvolvimento**, visando otimizar a produtividade e garantir o foco em projetos estratégicos.

## Canais de Entrada e Triagem
As solicitações chegam predominantemente via **E-mail**, sendo convertidas em tickets para acompanhamento. Para proteger o tempo de execução técnica, o fluxo segue a hierarquia de níveis abaixo:

| Nível | Grupo Responsável | Papel Principal |
| :--- | :--- | :--- |
| **N1** | **Suporte Geral / Help Desk** | Atendimento inicial, reset de senhas e orientações básicas. |
| **N2** | **Suporte a Sistemas** | **Triagem técnica obrigatória**. Validação de dados no RM/LDAP e identificação de falhas de processo. |
| **N3** | **Desenvolvimento** | Resolução de bugs de código, falhas de integração e novas funcionalidades. |

---

## 🛡️ Diretrizes de Governança e Comunicação

Para manter a integridade do planejamento e a eficiência do time:

### 1. Centralização de Demandas Externas
Todas as solicitações originadas por outros grupos (Rede, Infraestrutura, Sistemas) ou gestões externas **devem ser obrigatoriamente direcionadas ao Supervisor de Desenvolvimento (Marcelo)**. 
-   **Regra de Ouro:** Não deve haver solicitações diretas aos analistas desenvolvedores sem o conhecimento e priorização da supervisão.
-   **Impacto:** O acionamento direto desestabiliza o planejamento semanal, gera retrabalho e fragmenta o foco da equipe.

### 2. Triagem Prévia (Filtro N2)
O time de desenvolvimento só assume uma demanda após a confirmação pelo N2 (Suporte a Sistemas) de que o problema reside no código ou na lógica de integração, e não em inconsistências de dados no sistema de origem (RM/Totvs).

### 3. Registro de Atividades
Mesmo as demandas urgentes ou solicitações de gestores devem ser registradas formalmente no canal de atendimento para garantir a rastreabilidade e a transparência do trabalho realizado.

---

## 🔍 Fluxo de Diagnóstico: Funcional vs. Técnico

Para demandas que envolvem a otimização ou implantação de módulos do ERP (ex: Módulo de Contratos, Gestão de Frotas), seguimos o fluxo de maturidade abaixo:

1.  **Diagnóstico Funcional (N2 - Suporte a Sistemas):**
    *   **Ação:** Analisar se o problema é falta de treinamento, parametrização incorreta ou se o processo de negócio não se encaixa no padrão nativo da TOTVS.
    *   **Resultado esperado:** Um relatório ou parecer indicando se o RM atende nativamente ou se há um "gap" (buraco) de funcionalidade.

2.  **Definição Estratégica (Supervisão - Marcelo):**
    *   **Ação:** Validar o parecer do N2. Decidir se a solução será uma **mudança de processo no RM** (Funcional) ou se exigirá **desenvolvimento customizado** (Técnico, ex: Integração com Fluig).

3.  **Desenvolvimento de Solução (N3 - Dev):**
    *   **Ação:** Somente após a definição do item anterior, o N3 assume a demanda para criar integrações, Fórmulas Visuais complexas ou processos no Fluig.
    *   **Objetivo:** O desenvolvedor trabalha com requisitos claros e não em "tentativa e erro" funcional do ERP.

---

## Matriz de Responsabilidades (RACI)

| Atividade | N1 (Geral) | N2 (Sistemas) | N3 (Dev) |
| :--- | :---: | :---: | :---: |
| Monitorar Canais de Entrada | **R** | **A** | **C** |
| Validar Inconsistência de Dados | **C** | **R** | **I** |
| Analisar Bug de Código / Integração | **I** | **C** | **R** |
| Autorizar Novas Funcionalidades | **I** | **I** | **A (Marcelo)** |
| Manutenção de Servidores de Aplicação | **I** | **C** | **R*** |
| Atualização de Plataformas (Fluig, etc.) | **I** | **I** | **R*** |

*Legenda: **R** (Responsável), **A** (Aprova/Presta Contas), **C** (Consultado), **I** (Informado).*
***(\*) Dependência de Infraestrutura:** A manutenção técnica e atualização são do Desenvolvimento (N3), mas dependem da estabilidade e recursos (VM, Snapshot, SO, Rede) providos pelo setor de Infraestrutura.*

---
*Este processo formaliza a atuação do Grupo de Desenvolvimento como um time de engenharia, e não apenas suporte reativo.*
