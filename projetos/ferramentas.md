# Catálogo de Sistemas e Produtos (Visão Global 2025/2026)

Este documento consolida o mapeamento de ativos de tecnologia da Uniarp, integrando repositórios internos, plataformas de terceiros e fluxos de integração.

> **Nota Estratégica:** A maioria das integrações atuais opera sob o [Portal de Ensino (MVC)](https://github.com/uniarpdev/app-portal-mvc), com exceção da **Integração Avalia** (.NET Framework) e da **Minha Biblioteca** (PHP), que residem em ambientes separados. Existe um planejamento para a unificação futura no **Portal de Integrações**.

## 1. Gestão de Identidade e Acesso (IAM)
*Controle de autenticação, usuários e segurança institucional.*

| Produto | Repositório / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Identidade (Adm)** | [`app-ldap`](https://github.com/uniarpdev/app-ldap) | Gerenciamento administrativo de usuários LDAP (Desktop) | Marcelo |
| **Identidade (Web)** | [`app-ldap`](https://github.com/uniarpdev/app-ldap) | Interface de autosserviço e sincronismo AD (Web) | Marcelo |
| **Portaria (Gestão)** | [`app-portaria`](https://github.com/uniarpdev/app-portaria) | Gestão de acesso e integração RM (Desktop) | Marcelo |
| **Crachás (Web)** | [`app-portaria`](https://github.com/uniarpdev/app-portaria) | Solicitação de crachás por alunos/professores (Web) | Marcelo |
| **Suricato** | Telemática | Gestão de segurança física e controle de acesso | (Terceiro) |

## 2. Portais e Experiência do Aluno
*Ecossistema de interfaces e interação com o público acadêmico.*

| Produto | Repositório / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Portal de Ensino** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Portal intranet principal da Uniarp | Marcelo |
| **Carteirinha (Aluno)**| [`app-carteirinha`](https://github.com/uniarpdev/app-carteirinha) | Exibição digital de carteirinhas (Web) | Thiago |
| **Carteirinha (Adm)** | [`app-carteirinha`](https://github.com/uniarpdev/app-carteirinha) | Gestão e lotes de produção (Desktop) | Thiago |
| **Extrato de Notas** | [`app-extrato-notas`](https://github.com/uniarpdev/app-extrato-notas) | Consulta de notas (Colégio de Aplicação) | Felipe |
| **Monitoria** | PHP / Web | Gestão de agendamento de monitorias | Thiago |
| **Site Institucional** | WordPress | Site público uniarp.edu.br | Andre |
| **Portal de Eventos** | PHP / Web | SEDEPEX (Submissão/Avaliação) e Eventos Teatro | Andre |
| **Portais Diversos** | PHP / Web | Egresso, Jogos, Acervo Digital e LGPD (Parcial) | Andre |

## 3. Gestão Acadêmica e Integrações (Core ERP)
*Sistemas de processamento acadêmico e fluxos de integração de notas/matrículas.*

| Produto | Repositório / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **TOTVS RM** | ERP (C# / SQL) | Sistema Core (Educacional, Financeiro, RH, etc.) | **Rolff** |
| **Integrador Acad.** | [`app-academico`](https://github.com/uniarpdev/app-academico) | Automação de bolsas e processos RM (Console) | Marcelo |
| **Notas (Manager)** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Sincronismo LXP -> RM (Nova integração Grupo A) | Marcelo |
| **Notas (Avalia)** | .NET Framework | Integração antiga Avalia -> RM (Projeto Separado) | Marcelo |
| **Biblioteca Digital**| `Minha Biblioteca` (PHP) | Integração usuários RM -> Grupo A (Projeto Separado) | Marcelo |
| **Módulo Valorizza** | [`app-valorizza`](https://github.com/uniarpdev/app-valorizza) | Integração Valorizza (Reside no Portal de Ensino) | Marcelo |
| **Custom RM (Low)** | Fórmulas Visuais | Lógica interna e gatilhos de eventos do ERP | Marcelo |

## 4. Processos Administrativos e Backoffice
*Automação de fluxos internos, RH e atendimento.*

| Produto | Repositório / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Gestão de Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Painel administrativo e concessão (Desktop) | Thiago |
| **Inscrição Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Portal de inscrição para alunos (Web) | Thiago |
| **Pagamentos Med** | [`app-pagmed`](https://github.com/uniarpdev/app-pagmed) | Gestão de pagamentos curso de Medicina | Thiago |
| **RH e Férias** | [`app-aviso-ferias`](https://github.com/uniarpdev/app-aviso-ferias) | Emissão de avisos e recibos (Desktop) | Marcelo |
| **Gestão de Frotas** | [`app-gestao-frotas`](https://github.com/uniarpdev/app-gestao-frotas) | Controle de veículos (Bubble/Interno) | Thiago |
| **Processos BPM** | `Fluig` | Gestão de workflows e aprovações digitais | Theo |
| **Gestão de TI** | `GLPI` | Gerenciamento de chamados e ativos | Marcelo |

## 5. Bibliotecas e Utilitários (Helpers)
*Componentes de suporte e bibliotecas de classes compartilhadas.*

| Helper | Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **API TOTVS** | [`lib-api-totvs`](https://github.com/uniarpdev/lib-api-totvs) | Cliente de integração com APIs TOTVS | Marcelo |
| **API LDAP** | [`lib-api-ldap`](https://github.com/uniarpdev/lib-api-ldap) | Biblioteca de comunicação com servidor LDAP | Marcelo |
| **API Grupo A** | [`lib-api-grupoa`](https://github.com/uniarpdev/lib-api-grupoa) | Conector para APIs GrupoA-MaisCampus | Marcelo |
| **API Valorizza** | [`lib-api-valorizza`](https://github.com/uniarpdev/lib-api-valorizza) | Conector para APIs da Valorizza | Marcelo |
| **Dotnet Utils** | [`lib-dotnet-utils`](https://github.com/uniarpdev/lib-dotnet-utils) | Helpers gerais para projetos .NET C# | Marcelo |
| **Scripts & Tasks** | [`uniarpTasks`](https://github.com/uniarpdev/uniarpTasks) | Automações e tarefas agendadas | Marcelo |

## 6. Analytics e Automação de Escritório
*Inteligência de dados e ferramentas de produtividade.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Dashboards BI** | `Power BI` | Painéis estratégicos (RM/Fluig/Bolsas) | Marcelo/Thiago |
| **Office 365** | Power Automate | Automações de formulários e fluxos internos | Dionathan |
| **Impressão** | `SafePrint` | Gestão de cotas e filas de impressão | (Terceiro) |

## 7. Expansão e Colaboração (TI Uniarp)
Este repositório de documentação (`team-docs`) está em processo de expansão para cobrir as necessidades de **toda a equipe de TI da Uniarp**. 
- **Setor de Redes e Infraestrutura:** Futura inclusão de topologias, manuais de servidores e ativos de rede.
- **Suporte a Sistemas:** Centralização de manuais funcionais e base de conhecimento.

---
*Nota: Este catálogo reflete o levantamento oficial de 2025 consolidado com o planejamento de 2026.*
