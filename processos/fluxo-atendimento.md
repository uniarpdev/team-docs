# Fluxo de Atendimento e Suporte (GLPI)

Este documento define o processo de gestão de chamados para o **Grupo de Desenvolvimento**, visando otimizar o tempo da equipe e garantir que os analistas foquem em evolução de software e integrações.

## Estrutura de Atendimento em Níveis

Para proteger a produtividade do time de desenvolvimento, o fluxo de suporte deve seguir a hierarquia de níveis abaixo:

| Nível | Grupo Responsável | Papel Principal |
| :--- | :--- | :--- |
| **N1** | **Suporte Geral / Help Desk** | Atendimento inicial, reset de senhas e orientações de uso básico. |
| **N2** | **Suporte a Sistemas** | Triagem técnica, validação de dados no RM/LDAP e identificação de falhas de processo. |
| **N3** | **Desenvolvimento** | Correção de bugs no código, manutenção de APIs e novas integrações (RM -> LDAP -> Portal -> GLPI). |

## Fluxo de Escalonação

1.  **Abertura:** O usuário abre o chamado no GLPI selecionando a categoria do sistema.
2.  **Triagem (N2):** O grupo de **Suporte a Sistemas** realiza a primeira análise técnica.
    -   *Se for erro de cadastro ou processo:* O N2 resolve e encerra o chamado.
    -   *Se for falha na integração ou erro de código:* O N2 escala o chamado para o grupo **Desenvolvimento**.
3.  **Resolução (N3):** O analista de desenvolvimento atua na correção técnica e devolve o chamado para o N2 validar com o usuário.

## Matriz de Responsabilidades (RACI)

| Atividade | N1 (Geral) | N2 (Sistemas) | N3 (Dev) |
| :--- | :---: | :---: | :---: |
| Monitorar fila do GLPI | **R** | **A** | **C** |
| Reset de senha LDAP/Portal | **R** | **A** | **I** |
| Validar dados no RM/Totvs | **C** | **R** | **I** |
| Corrigir bugs em sistemas internos | **I** | **C** | **R** |
| Manutenção do Servidor GLPI | **I** | **C** | **R*** |
| Customização de Plugins GLPI | **I** | **I** | **R** |

*Legenda: **R** (Responsável), **A** (Aprova/Presta Contas), **C** (Consultado), **I** (Informado).*
*\*Nota: A manutenção do servidor GLPI é feita pelo Dev atualmente, mas o objetivo é migrar para Infra.*

## Diretrizes de Atendimento para o Dev

-   **Não atender chamados sem triagem:** O time de desenvolvimento não deve assumir chamados que não passaram pelo N2 (Suporte a Sistemas).
-   **Documentação:** Sempre que um erro de integração for resolvido, a solução deve ser documentada na **Base de Conhecimento** do GLPI para que o N2 possa resolver futuramente sem escalonar.
-   **Ponto Focal:** O Supervisor (Marcelo) valida a necessidade de desenvolvimento antes do analista iniciar a codificação de uma nova funcionalidade solicitada via chamado.

---
*Este processo visa reduzir a carga reativa do Grupo de Desenvolvimento, permitindo foco em projetos estratégicos.*
