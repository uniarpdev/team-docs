# Catálogo de Sistemas e Produtos (Visão Global 2025/2026)

Este documento consolida o mapeamento de ativos de tecnologia da Uniarp, integrando repositórios internos, plataformas de terceiros e fluxos de integração.

## 1. Gestão de Identidade e Acesso (IAM)
*Controle de autenticação, usuários e segurança institucional.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Identidade (Adm)** | `app-ldap` | Gestão administrativa de usuários LDAP (Desktop) | Marcelo |
| **Identidade (Web)** | `app-ldap` / `lib-api-ldap` | Interface de autosserviço e sincronismo AD (Web) | Marcelo |
| **Portaria (Gestão)** | `app-portaria` | Gestão de acesso e integração RM (Desktop) | Marcelo |
| **Crachás (Web)** | `app-portaria` | Solicitação de crachás por alunos/professores (Web) | Marcelo |
| **Suricato** | Telemática | Gestão de segurança física e controle de acesso | (Terceiro) |

## 2. Portais e Experiência do Aluno
*Ecossistema de interfaces e interação com o público acadêmico.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Portal de Ensino** | `app-portal-mvc` | Portal intranet principal da Uniarp | Marcelo |
| **Portal Educacional**| Totvs (RM) | Interface nativa RM para professores e alunos | (Terceiro) |
| **Minha Uniarp (App)**| Totvs (Mobile) | Aplicativo mobile para informações acadêmicas | (Terceiro) |
| **Carteirinha (Aluno)**| `app-carteirinha` | Exibição digital de carteirinhas (Web) | Thiago |
| **Carteirinha (Adm)** | `app-carteirinha` | Gestão e lotes de produção (Desktop) | Thiago |
| **Extrato de Notas** | `app-extrato-notas` | Consulta de notas (Colégio de Aplicação) | Felipe |
| **Monitoria** | `Monitoria` | Gestão de agendamento de monitorias | Thiago |
| **Site Institucional** | WordPress | Site público uniarp.edu.br | Andre |
| **Portal de Eventos** | PHP/Web | SEDEPEX (Submissão/Avaliação) e Eventos Teatro | Andre |
| **Portais Diversos** | PHP/Web | Egresso, Jogos, Acervo Digital e LGPD (Parcial) | Andre |

## 3. Gestão Acadêmica e Integrações (Core ERP)
*Sistemas de processamento acadêmico e fluxos de integração de notas/matrículas.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **TOTVS RM** | ERP (C# / SQL) | Sistema Core (Educacional, Financeiro, RH, etc.) | Marcelo |
| **Integrador Acad.** | `app-academico` | Automação de bolsas e processos RM (Console) | Marcelo |
| **Plataforma A (LXP)**| Grupo A | Ambiente Virtual de Aprendizagem (LXP/LTI) | (Terceiro) |
| **Integração Notas** | `lib-api-grupoa` | Sincronismo LXP -> RM e Avalia -> RM | Marcelo |
| **Biblioteca Digital**| `Minha Biblioteca` | Integração de usuários RM -> Grupo A | Marcelo |
| **Módulo Valorizza** | `app-valorizza` | Integração com a plataforma Valorizza | Marcelo |
| **Custom RM (Low)** | Fórmulas Visuais | Lógica interna e gatilhos de eventos do ERP | Marcelo |

## 4. Processos Administrativos e Backoffice
*Automação de fluxos internos, RH e atendimento.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Gestão de Bolsas** | `app-bolsas` | Inscrição (Web) e Gestão de Bolsas (Desktop) | Thiago |
| **Pagamentos Med** | `app-pagmed` | Gestão de pagamentos curso de Medicina | Thiago |
| **RH e Férias** | `app-aviso-ferias` | Emissão de avisos e recibos (Meu RH Totvs) | Marcelo |
| **Gestão de Frotas** | `app-gestao-frotas` | Controle de veículos (Bubble/Interno) | Thiago |
| **Processos BPM** | `Fluig` | Gestão de workflows e aprovações digitais | Theo |
| **Gestão de TI** | `GLPI` | Gerenciamento de chamados e ativos | Marcelo |
| **GED / Diplomas** | `DocXpress` | Digitalização e gestão de diplomas digitais | (Terceiro) |
| **CRM / Marketing** | `Rubeus` | Gestão de captação e relacionamento | (Terceiro) |
| **Ponto / RH** | `Kairos` (Dimep) | Coleta de registros de ponto eletrônico | (Terceiro) |

## 5. Analytics e Automação de Escritório
*Inteligência de dados e ferramentas de produtividade.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Dashboards BI** | `Power BI` | Painéis estratégicos (RM/Fluig/Bolsas) | Marcelo/Thiago |
| **Office 365** | Power Automate | Automações de formulários e fluxos internos | Dionathan |
| **Impressão** | `SafePrint` | Gestão de cotas e filas de impressão | (Terceiro) |

## 6. Candidatos a Arquivamento / Desativação
*Sistemas legados ou duplicados aguardando análise para descontinuação.*

| Produto | Tecnologia | Motivo |
| :--- | :--- | :--- |
| **uniarpApps** | Diversas | Repositório monólito sendo fatiado em apps próprios |
| **Moodle** | EaD | Sendo substituído/complementado pelo LXP |

---
*Nota: Este catálogo reflete o levantamento oficial de 2025 consolidado com o planejamento de 2026.*
