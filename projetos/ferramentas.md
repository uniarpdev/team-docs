# Catálogo de Sistemas e Produtos (Visão Global)

Este documento mapeia os ativos de tecnologia da Uniarp por **Produto/Sistema**, consolidando repositórios, bibliotecas, plataformas de terceiros e customizações internas.

## 1. Gestão de Identidade e Acesso (IAM)
*Sistemas que controlam a autenticação e autorização institucional.*

| Produto | Repositórios / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Identidade (Adm)** | `app-ldap` | Gerenciamento administrativo de usuários LDAP (Desktop) | Marcelo |
| **Identidade (Web)** | `app-ldap` / `lib-api-ldap` | Interface de autosserviço para usuários (Web) | Marcelo |
| **Portaria (Gestão)** | `app-portaria` | Monitoramento e gestão de acesso (Desktop) | Marcelo |
| **Crachás (Web)** | `app-portaria` | Solicitação de crachás por alunos/professores (Web) | Marcelo |

## 2. Portais e Experiência do Aluno
*Interfaces de interação direta com o corpo discente e público externo.*

| Produto | Repositórios / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Portal de Ensino** | `app-portal-mvc` | Portal intranet principal da Uniarp | Marcelo |
| **Carteirinha (Aluno)**| `app-carteirinha` | Exibição digital de carteirinhas estudantis (Web) | Thiago |
| **Carteirinha (Adm)** | `app-carteirinha` | Impressão e gestão administrativa (Desktop) | Thiago |
| **Extrato de Notas** | `app-extrato-notas` | Emissão de extratos (Colégio de Aplicação) | Thiago |
| **Site Institucional** | WordPress (`Portal Uniarp`) | Site público uniarp.edu.br | Andre |

## 3. Gestão Acadêmica e Integrações ERP (TOTVS RM)
*Núcleo de processamento de dados e automações do ecossistema acadêmico.*

| Produto | Repositórios / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Integrador Acadêmico**| `app-academico` / `lib-api-totvs` | Automação e integração direta com RM | Marcelo |
| **Integração de Notas** | `Integração Avalia` / `lib-api-grupoa` | Sincronismo de notas (Avalia/Grupo A) | Marcelo |
| **Biblioteca Digital** | `Minha Biblioteca` | Integração com acervo digital (PHP) | Marcelo |
| **Módulo Valorizza** | `app-valorizza` / `lib-api-valorizza`| Integração com a plataforma Valorizza | Marcelo |
| **Custom RM (Low)** | Fórmulas Visuais, SQL, ETL | Lógica interna e gatilhos do ERP | Marcelo |

## 4. Processos Administrativos e Backoffice
*Sistemas de suporte interno e automação de fluxos de trabalho.*

| Produto | Repositórios / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Gestão de Bolsas** | `app-bolsas` | Painel administrativo e concessão (Desktop) | Thiago |
| **Inscrição de Bolsas**| `app-bolsas` | Formulário de inscrição para alunos (Web) | Thiago |
| **Pagamentos Med** | `app-pagmed` | Gestão de pagamentos curso de Medicina (Desktop) | Thiago |
| **RH e Férias** | `app-aviso-ferias` | Emissão de avisos de férias (Desktop) | Thiago |
| **Gestão de Frotas** | `app-gestao-frotas` / `Bubble.io` | Controle de veículos e solicitações | Thiago |
| **Processos BPM** | Plataforma `Fluig` | Fluxos de trabalho e aprovações digitais | Theo |
| **Gestão de TI** | `GLPI` / `team-docs` | Chamados, Inventário e Documentação | Marcelo |

## 5. Analytics e Inteligência de Dados (BI)
*Extração e visualização de dados estratégicos.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Dashboards Uniarp** | `Power BI` | Painéis gerenciais e monitoramento | Marcelo/Thiago |

## 6. Infraestrutura de Código e Componentes (Libs)
*Arquiteturas de suporte que atendem a múltiplos produtos.*

| Componente | Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **API de Serviços** | `app-portal-api` / `app-portal-web` | Camada de abstração e web-services | Marcelo |
| **Dotnet Utils** | `lib-dotnet-utils` | Utilitários e helpers para projetos C# | Marcelo |
| **Scripts & Tasks** | `uniarpTasks` | Automações rápidas e tarefas agendadas | Marcelo |

## 7. Candidatos a Arquivamento / Desativação
*Sistemas legados ou duplicados aguardando análise para descontinuação.*

| Produto | Repositório | Motivo |
| :--- | :--- | :--- |
| *(Em análise)* | | |

---
*Nota: Para novos sistemas, siga o padrão de nomenclatura `app-`, `lib-` ou `bpm-`.*
