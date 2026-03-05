# Ferramentas e Pontos Focais

Este documento mapeia os principais repositórios da organização **uniarpdev** e identifica os pontos focais para manutenção e suporte.

## Definição de Papéis

Para todos os projetos listados abaixo, a estrutura de responsabilidade segue este padrão:

-   **Supervisão e Regras de Negócio (Marcelo):** Responsável pela definição da arquitetura, levantamento de requisitos junto às áreas solicitantes e validação das regras de negócio.
-   **Ponto Focal (Analista/Supervisor):** Responsável pela execução técnica, codificação, manutenção evolutiva e atendimento de chamados (GLPI) relacionados à ferramenta.

## Aplicações Ativas (Apps)
Sistemas em produção ou desenvolvimento constante.

| Repositório | Descrição | Plataforma | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **app-portal-mvc** | Portal intranet Uniarp | Web | Marcelo |
| **app-academico** | Integrador Acadêmico: Automação TOTVS RM | Console | Marcelo |
| **app-bolsas** | Gestão de bolsas da Uniarp | Web/Desktop | Thiago |
| **app-carteirinha** | Gestão de carteirinhas estudantis | Web/Desktop | Thiago |
| **app-pagmed** | Gestão de pagamentos (Curso de Medicina) | Desktop | Thiago |
| **app-extrato-notas** | Emissão de extratos (Colégio de Aplicação) | Desktop | Thiago |
| **app-aviso-ferias** | Sistema para envio de aviso de férias | Desktop | Thiago |
| **app-portaria** | Sistema de solicitação de crachás | Web/Desktop | Marcelo |

## Projetos em Planejamento ou Testes
Projetos que ainda não foram iniciados ou são ambientes de teste.

| Repositório | Descrição | Status | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **app-gestao-frotas** | Controle de solicitações de veículos | Planejamento | |
| **app-portal-api** | API de processos internos sistemas uniarp | API | Marcelo |
| **app-portal-web** | Interface web para consumo API de integrações | Web | Marcelo |
| **app-valorizza** | Integração com a plataforma Valorizza | Planejamento | Marcelo |

## Bibliotecas (Libs)
Componentes compartilhados e integrações de baixo nível.

| Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- |
| **lib-api-ldap** | API para integração com LDAP | Marcelo |
| **lib-api-totvs** | Biblioteca de classes para APIs da Totvs | Marcelo |
| **lib-api-grupoa** | Cliente .NET para APIs GrupoA-MaisCampus | Marcelo |
| **lib-api-valorizza** | Biblioteca de integração com Valorizza | Marcelo |
| **lib-dotnet-utils** | Utilitários para projetos dotnet c# | Marcelo |

## Plataformas e Terceiros
Soluções de terceiros, BPM, Low-Code e desenvolvimentos fora do Git.

| Ferramenta | Descrição | Plataforma | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Fluig** | Implementações e processos sobre a plataforma Fluig | BPM / Low-Code | Theo |
| **Power BI** | Desenvolvimento de dashboards e relatórios gerenciais | BI / Analytics | Marcelo/Thiago |
| **Portal Uniarp** | Site institucional da Uniarp (WordPress) | CMS / Web | Andre |
| **Bubble.io** | Gestão de frotas e monitoria (No-Code) | Web / No-Code | Thiago |
| **GLPI** | Sistema de chamados (Manutenção e Customização) | ITSM / PHP | Marcelo |
| **Integração Avalia** | Integração de notas (Projeto fora do Git) | .NET Framework | Marcelo |
| **Minha Biblioteca**| Integração com acervo digital (Plano de migração para API) | PHP | Marcelo |

## Outros Projetos Relevantes
| Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- |
| **uniarpTasks** | Scripts de integração e tarefas agendadas | Marcelo |
| **team-docs** | Documentação do time de desenvolvimento | Marcelo |

## Customizações e Ferramentas Internas (TOTVS RM)
Componentes de desenvolvimento "low-code" e lógica de negócio dentro do ERP.

| Ferramenta | Descrição | Responsabilidade Técnica |
| :--- | :--- | :--- |
| **Fórmulas Visuais** | Gatilhos e automações de processos no RM | Desenvolvimento (Regra/Arquitetura) |
| **Consultas SQL** | Views e Scripts para Relatórios e Cubos | Desenvolvimento (Performance/Lógica) |
| **Integração ETL** | Fluxos de extração e carga de dados (Conceitos) | Desenvolvimento |
| **Metadados** | Criação de tabelas e campos customizados | Desenvolvimento/Suporte |
| **Gerador de Saídas** | Layouts de integração bancária e fiscal | Suporte (Parametrização) |

---
*Nota: Para novos projetos, siga o padrão de nomenclatura `app-`, `lib-` ou `bpm-`.*
