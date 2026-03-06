# Catálogo de Sistemas e Produtos (Visão Global 2025/2026)

Este documento consolida o mapeamento de ativos de tecnologia da Uniarp, integrando repositórios internos, plataformas de terceiros e fluxos de integração.

> **Nota Estratégica:** A maioria das integrações atuais opera sob o [Portal de Ensino (MVC)](https://github.com/uniarpdev/app-portal-mvc), com exceção da **Integração Avalia** (.NET Framework) e da **Minha Biblioteca** (PHP), que residem em ambientes separados. Existe um planejamento para a unificação futura no **Portal de Integrações**.

## 1. Gestão de Identidade e Acesso (IAM)
*Controle de autenticação, usuários e segurança institucional.*

| Produto | Repositório / Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Identidade (Adm)** | [`app-ldap`](https://github.com/uniarpdev/app-ldap) | Interno | Gestão de usuários LDAP (Desktop) | Marcelo |
| **Identidade (Web)** | [`app-ldap`](https://github.com/uniarpdev/app-ldap) | Interno | Interface de autosserviço LDAP (Web) | Marcelo |
| **Portaria (Gestão)** | [`app-portaria`](https://github.com/uniarpdev/app-portaria) | Interno | Gestão de acesso e integração RM (Desktop) | Marcelo |
| **Crachás (Web)** | [`app-portaria`](https://github.com/uniarpdev/app-portaria) | Interno | Solicitação de crachás (Web) | Marcelo |
| **Suricato** | Telemática | Terceiro | Gestão de segurança física e acesso | Marcelo |

## 2. Portais e Experiência do Aluno
*Ecossistema de interfaces e interação com o público acadêmico.*

| Produto | Repositório / Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Portal de Ensino** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Interno | Portal intranet principal da Uniarp | Marcelo |
| **Portal Educacional**| Totvs (RM) | Terceiro | Interface nativa RM (Alunos/Prof) | Rolff |
| **Minha Uniarp (App)**| Totvs (Mobile) | Terceiro | Aplicativo mobile acadêmico | Rolff |
| **Carteirinha (Alu)**| [`app-carteirinha`](https://github.com/uniarpdev/app-carteirinha) | Interno | Exibição digital de carteirinhas (Web) | Thiago |
| **Carteirinha (Adm)** | [`app-carteirinha`](https://github.com/uniarpdev/app-carteirinha) | Interno | Gestão e lotes de produção (Desktop) | Thiago |
| **Extrato de Notas** | [`app-extrato-notas`](https://github.com/uniarpdev/app-extrato-notas) | Interno | Consulta de notas (Colégio de Aplicação) | Thiago |
| **Monitoria** | `Bubble.io` | Terceiro | Gestão de agendamento de monitorias | Thiago |
| **Site Institucional** | WordPress | Terceiro | Site público uniarp.edu.br | Andre |
| **Portal de Eventos** | PHP / Web | Interno | SEDEPEX e Eventos Teatro | Andre |
| **Portais Diversos** | PHP / Web | Interno | Egresso, Jogos, Acervo e LGPD | Andre |

## 3. Gestão Acadêmica e Integrações (Core ERP)
*Sistemas de processamento acadêmico e fluxos de integração.*

| Produto | Repositório / Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **TOTVS RM** | ERP (C# / SQL) | Terceiro | Sistema Core Institucional | **Rolff** |
| **Integrador Acad.** | [`app-academico`](https://github.com/uniarpdev/app-academico) | Interno | Automação de processos RM (Console) | Marcelo |
| **Notas (Manager)** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Interno | Sincronismo LXP -> RM (Portal) | Marcelo |
| **Notas (Avalia)** | .NET Framework | Interno | Integração antiga Avalia -> RM | Marcelo |
| **Biblioteca Dig.** | `Minha Biblioteca` (PHP) | Interno | Integração usuários RM -> Grupo A | Marcelo |
| **Módulo Valorizza** | [`app-valorizza`](https://github.com/uniarpdev/app-valorizza) | Interno | Integração Valorizza (Portal) | Marcelo |
| **Custom RM (Low)** | Fórmulas Visuais | Interno | Lógica interna e gatilhos do ERP | Marcelo |

## 4. Processos Administrativos e Backoffice
*Automação de fluxos internos e suporte.*

| Produto | Repositório / Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Gestão de Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Interno | Painel administrativo (Desktop) | Thiago |
| **Inscrição Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Interno | Portal de inscrição para alunos (Web) | Thiago |
| **Pagamentos Med** | [`app-pagmed`](https://github.com/uniarpdev/app-pagmed) | Interno | Gestão de pagamentos curso Medicina | Thiago |
| **RH e Férias** | [`app-aviso-ferias`](https://github.com/uniarpdev/app-aviso-ferias) | Interno | Emissão de avisos e recibos (Desktop) | Marcelo |
| **Gestão de Frotas** | [`app-gestao-frotas`](https://github.com/uniarpdev/app-gestao-frotas) | Interno | Controle de veículos (Bubble/Interno) | Thiago |
| **Processos BPM** | `Fluig` | Terceiro | Gestão de workflows e aprovações | Theo |
| **Gestão de TI** | `GLPI` | Terceiro | Gerenciamento de chamados e ativos | Marcelo |

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

| Produto | Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Dashboards BI** | `Power BI` | Terceiro | Painéis estratégicos (RM/Fluig) | Marcelo/Thiago |
| **Office 365** | Power Automate | Terceiro | Automações de formulários/fluxos | Dionathan |
| **Impressão** | `SafePrint` | Terceiro | Gestão de cotas de impressão | Dionathan |

## 7. Expansão e Colaboração (TI Uniarp)
Este repositório de documentação (`team-docs`) está em processo de expansão para cobrir as necessidades de **toda a equipe de TI da Uniarp**. 
- **Setor de Redes e Infraestrutura:** Futura inclusão de topologias e manuais de servidores.
- **Suporte a Sistemas:** Centralização de manuais funcionais e base de conhecimento.

---
*Nota: Este catálogo reflete o levantamento oficial de 2025 consolidado com o planejamento de 2026.*
