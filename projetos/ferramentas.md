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
| **Sincronismo AD** | Integração RM -> AD | Interno | Manutenção de usuários no Active Directory | Marcelo |
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
| **Atendimento Whats** | WorkChat | Terceiro | Automação via WhatsApp | A definir |
| **Gestão Carreira** | WorkAlove | Terceiro | Plataforma de gestão de carreira | A definir |
| **Site Institucional** | WordPress | Terceiro | Site público uniarp.edu.br | Andre |
| **Portal de Eventos** | PHP / Web | Interno | SEDEPEX e Eventos Teatro | Andre |
| **Portais Diversos** | PHP / Web | Interno | Egresso, Jogos, Acervo e LGPD | Andre |

## 3. Ecossistema TOTVS RM (Módulos e Customizações)
*Vertical de gestão institucional (ERP). Supervisão Geral: **Rolff***

| Módulo / Produto | Tecnologia | Origem | Descrição | Analista Responsável |
| :--- | :--- | :--- | :--- | :--- |
| **Educacional** | RM Classis Net | Terceiro | Gestão acadêmica e enturmação | A definir |
| **Financeiro** | RM Fluxus | Terceiro | Gestão de contas a pagar/receber e caixa | A definir |
| **Contábil / Fiscal**| RM Saldus / Liber | Terceiro | Escrituração, impostos e contabilidade | A definir |
| **Folha / RH** | RM Labore / Vitae | Terceiro | Gestão de pessoas e pagamentos | A definir |
| **Ponto Eletrônico** | RM Chronus | Terceiro | Gestão de jornada e integração Kairos | A definir |
| **Estoque / Compras** | RM Nucleus | Terceiro | Suprimentos, faturamento e compras | A definir |
| **Biblioteca** | RM Biblios | Terceiro | Gestão de acervo físico e empréstimos | A definir |
| **Segurança / Saúde** | RM Agilis / Bonum | Terceiro | Atendimento e gestão patrimonial | A definir |
| **Custom RM (Low)** | Fórmulas Visuais | Interno | Lógica interna e gatilhos do ERP | Marcelo |

## 4. Integrações Acadêmicas e de Dados
*Fluxos de comunicação entre o RM e plataformas externas.*

| Produto | Repositório / Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Integrador Acad.** | [`app-academico`](https://github.com/uniarpdev/app-academico) | Interno | Automação de processos RM (Console) | Marcelo |
| **Notas (Manager)** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Interno | Sincronismo LXP -> RM (Portal) | Marcelo |
| **Notas (Avalia)** | .NET Framework | Interno | Integração antiga Avalia -> RM | Marcelo |
| **Biblioteca Dig.** | `Minha Biblioteca` (PHP) | Interno | Integração usuários RM -> Grupo A | Marcelo |
| **Módulo Valorizza** | Integração (Portal) | Interno | Integração Valorizza (Reside no Portal) | Marcelo |
| **Módulo Orbita** | Integração RM | Terceiro | Geração de matrículas (Orbita -> RM) | A definir |
| **Assinatura Digit.**| Sign (Totvs) | Terceiro | Assinatura eletrônica de documentos | A definir |

## 5. Processos Administrativos e Backoffice
*Automação de fluxos internos e suporte.*

| Produto | Repositório / Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Gestão de Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Interno | Painel administrativo (Desktop) | Thiago |
| **Inscrição Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Interno | Portal de inscrição para alunos (Web) | Thiago |
| **Pagamentos Med** | [`app-pagmed`](https://github.com/uniarpdev/app-pagmed) | Interno | Gestão de pagamentos curso Medicina | Thiago |
| **RH e Férias** | [`app-aviso-ferias`](https://github.com/uniarpdev/app-aviso-ferias) | Interno | Emissão de avisos e recibos (Desktop) | Marcelo |
| **Meu RH (App)** | Totvs (Mobile) | Terceiro | Gestão de comunicação com colaboradores | Rolff |
| **Gestão de Frotas** | [`app-gestao-frotas`](https://github.com/uniarpdev/app-gestao-frotas) | Interno | Controle de veículos (Bubble/Interno) | Thiago |
| **Processos BPM** | `Fluig` | Terceiro | Gestão de workflows e aprovações | Theo |
| **Gestão de TI** | `GLPI` | Terceiro | Gerenciamento de chamados e ativos | Marcelo |
| **CRM / Marketing** | Rubeus | Terceiro | Gestão de relacionamento e captação | A definir |
| **Ponto / RH** | Kairos (Dimep) | Terceiro | Coleta de registros de ponto | A definir |
| **GED / Diplomas** | DocXpress/Diplomax| Terceiro | Digitalização e gestão de diplomas | A definir |

## 6. Bibliotecas e Utilitários (Helpers)
*Componentes de suporte e bibliotecas de classes compartilhadas.*

| Helper | Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **API TOTVS** | [`lib-api-totvs`](https://github.com/uniarpdev/lib-api-totvs) | Cliente de integração com APIs TOTVS | Marcelo |
| **API LDAP** | [`lib-api-ldap`](https://github.com/uniarpdev/lib-api-ldap) | Biblioteca de comunicação com servidor LDAP | Marcelo |
| **API Grupo A** | [`lib-api-grupoa`](https://github.com/uniarpdev/lib-api-grupoa) | Conector para APIs GrupoA-MaisCampus | Marcelo |
| **API Valorizza** | [`lib-api-valorizza`](https://github.com/uniarpdev/lib-api-valorizza) | Conector para APIs da Valorizza | Marcelo |
| **Dotnet Utils** | [`lib-dotnet-utils`](https://github.com/uniarpdev/lib-dotnet-utils) | Helpers gerais para projetos .NET C# | Marcelo |
| **Scripts & Tasks** | [`uniarpTasks`](https://github.com/uniarpdev/uniarpTasks) | Automações e tarefas agendadas | Marcelo |

## 7. Analytics e Automação de Escritório
*Inteligência de dados e ferramentas de produtividade.*

| Produto | Tecnologia | Origem | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- | :--- |
| **Dashboards BI** | `Power BI` | Terceiro | Painéis estratégicos (RM/Fluig) | Marcelo/Thiago |
| **Office 365** | Power Automate | Terceiro | Automações de formulários/fluxos | Dionathan |
| **Impressão** | `SafePrint` | Terceiro | Gestão de cotas de impressão | Dionathan |

## 8. Expansão e Colaboração (TI Uniarp)
Este repositório de documentação (`team-docs`) está em processo de expansão para cobrir as necessidades de **toda a equipe de TI da Uniarp**. 
- **Setor de Redes e Infraestrutura:** Futura inclusão de topologias e manuais de servidores.
- **Suporte a Sistemas:** Centralização de manuais funcionais e base de conhecimento.

---
*Nota: Este catálogo reflete o levantamento oficial de 2025 consolidado com o planejamento de 2026.*
