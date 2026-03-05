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

## Matriz de Responsabilidades (RACI)

| Atividade | N1 (Geral) | N2 (Sistemas) | N3 (Dev) |
| :--- | :---: | :---: | :---: |
| Monitorar Canais de Entrada | **R** | **A** | **C** |
| Validar Inconsistência de Dados | **C** | **R** | **I** |
| Analisar Bug de Código / Integração | **I** | **C** | **R** |
| Autorizar Novas Funcionalidades | **I** | **I** | **A (Marcelo)** |
| Manutenção de Servidores de Aplicação | **I** | **C** | **R*** |

*Legenda: **R** (Responsável), **A** (Aprova/Presta Contas), **C** (Consultado), **I** (Informado).*
***(\*) Dependência de Infraestrutura:** A manutenção técnica da aplicação é do Desenvolvimento (N3), mas depende da estabilidade e recursos (VM, SO, Rede) providos pelo setor de Infraestrutura.*

---
*Este processo formaliza a atuação do Grupo de Desenvolvimento como um time de engenharia, e não apenas suporte reativo.*
