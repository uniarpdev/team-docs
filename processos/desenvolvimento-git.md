# Padrões de Desenvolvimento e Git

Este documento define os padrões para o uso de Git e a estratégia de branching adotada pelo Grupo de Desenvolvimento Uniarp, visando manter o histórico limpo e organizado.

## 🚀 Estratégia de Branching

Toda nova implementação, seja ela documental ou técnica, deve ser realizada em uma nova branch isolada. O uso de commits diretos na branch principal (`main` ou `master`) é desencorajado.

### 🏷️ Prefixos de Branch
As branches devem ser nomeadas utilizando prefixos que indiquem claramente o propósito da alteração:

| Prefixo | Descrição | Exemplo |
| :--- | :--- | :--- |
| `feat/` | Nova funcionalidade ou recurso. | `feat/login-unico` |
| `fix/` | Correção de bugs ou erros em produção. | `fix/erro-calculo-media` |
| `docs/` | Alterações exclusivas na documentação. | `docs/fluxo-integracao` |
| `refactor/` | Melhoria no código sem alteração de funcionalidade. | `refactor/camada-servico` |
| `chore/` | Tarefas de manutenção, atualização de pacotes ou builds. | `chore/update-nuget-ldap` |

### 🔄 Fluxo de Trabalho (GitHub Flow)

Para garantir a qualidade do código e a integridade do ambiente de produção, seguimos um fluxo de trabalho baseado em revisão por pares:

1.  **Criação da Branch:** Toda alteração deve iniciar com a criação de uma branch a partir da `main`, utilizando os prefixos definidos acima.
2.  **Proibição de Push Direto:** **É estritamente proibido realizar push direto na branch `main`.** Todas as alterações devem passar pelo processo de revisão.
3.  **Pull Request (PR):** Ao finalizar o desenvolvimento, o desenvolvedor deve abrir um Pull Request para a branch `main`.
    *   O PR deve conter uma descrição clara do que foi implementado ou corrigido.
    *   Devem ser vinculados os cards do Planner ou tickets do GLPI correspondentes, se houver.
4.  **Análise e Revisão:** Todo PR deve ser analisado por outro membro da equipe ou pelo Supervisor antes de ser mergeado.
    *   **Critérios de Revisão:** Aderência aos padrões de código, presença de testes (se aplicável), documentação atualizada e ausência de efeitos colaterais.
5.  **Merge:** Após a aprovação (Approve), a branch pode ser integrada à `main`.

---
*Baseado nos padrões de governança do Grupo de Desenvolvimento Uniarp.*
