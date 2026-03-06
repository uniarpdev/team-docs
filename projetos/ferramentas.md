# Catálogo de Sistemas e Produtos (Visão Global 2025/2026)

Este documento consolida o mapeamento de ativos de tecnologia da Uniarp, separando o que é **Desenvolvimento Interno** do que é **Sustentação de Sistemas de Terceiros**.

---

## 🏗️ PARTE 1: DESENVOLVIMENTO INTERNO (Engenharia e Software)
*Ativos de tecnologia onde a Uniarp é proprietária da lógica, código ou implementação customizada.*

### 1.1. Portais e Aplicações Web/Desktop
| Produto | Repositório / Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Portal de Ensino** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Portal intranet principal da Uniarp | Marcelo |
| **Identidade (Adm)** | [`app-ldap`](https://github.com/uniarpdev/app-ldap) | Gestão administrativa de usuários LDAP (Desktop) | Marcelo |
| **Identidade (Web)** | [`app-ldap`](https://github.com/uniarpdev/app-ldap) | Interface de autosserviço LDAP (Web) | Marcelo |
| **Portaria & Crachás**| [`app-portaria`](https://github.com/uniarpdev/app-portaria) | Gestão de acesso e solicitação de crachás | Marcelo |
| **Gestão de Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Painel administrativo e concessão (Desktop) | Thiago |
| **Inscrição Bolsas** | [`app-bolsas`](https://github.com/uniarpdev/app-bolsas) | Portal de inscrição para alunos (Web) | Thiago |
| **Carteirinha (Alu)**| [`app-carteirinha`](https://github.com/uniarpdev/app-carteirinha) | Exibição digital de carteirinhas (Web) | Thiago |
| **Carteirinha (Adm)** | [`app-carteirinha`](https://github.com/uniarpdev/app-carteirinha) | Gestão e lotes de produção (Desktop) | Thiago |
| **Extrato de Notas** | [`app-extrato-notas`](https://github.com/uniarpdev/app-extrato-notas) | Consulta de notas (Colégio de Aplicação) | Thiago |
| **Pagamentos Med** | [`app-pagmed`](https://github.com/uniarpdev/app-pagmed) | Gestão de pagamentos curso Medicina | Thiago |
| **RH e Férias** | [`app-aviso-ferias`](https://github.com/uniarpdev/app-aviso-ferias) | Emissão de avisos e recibos (Desktop) | Marcelo |
| **Portais Diversos** | PHP / Web | SEDEPEX, Egresso, Jogos, Acervo e LGPD | Maia |
| **Monitoria** | `Bubble.io` | Gestão de agendamento de monitorias (No-Code) | Thiago |
| **Gestão de Frotas** | `Bubble.io` | Controle de veículos | Thiago |
| **Site Institucional** | WordPress | Site público uniarp.edu.br | Maia |

### 1.2. Funcionalidades - Portal de Ensino (MVC)
*Segmentação granular dos serviços disponíveis no portal unificado (Branch: unificacao).*

#### A. Módulo Acadêmico (Edu & Aluno)
| Funcionalidade | Descrição | Público |
| :--- | :--- | :--- |
| **Check-in Aula** | Registro de presença via portal com validação de geolocalização/horário. | Aluno |
| **Análise Curricular**| Emissão de relatórios de evolução no curso e matriz curricular. | Aluno |
| **Aproveitamento** | Fluxo digital para solicitação e acompanhamento de aproveitamento de estudos. | Aluno |
| **Gestão Acadêmica** | Consulta de notas, faltas, horários e documentos acadêmicos. | Aluno |
| **Painel Coord.** | Visualização e gestão de professores e turmas vinculadas. | Coordenador |

#### B. Módulo de Integrações (Middleware)
| Funcionalidade | Descrição | Status |
| :--- | :--- | :--- |
| **Gateway AVA** | Ponte de autenticação e sincronismo para ambientes LXP/Moodle. | Ativo |
| **Sync de Notas** | Motor de integração para retorno de avaliações externas ao TOTVS RM. | Ativo |
| **Módulo Valorizza**| Integração de dados de carreira e práticas acadêmicas. | Em Unificação |

#### C. Módulo de Suporte e Identidade
| Funcionalidade | Descrição | Público |
| :--- | :--- | :--- |
| **Self-Service ID** | Reset de senha e atualização cadastral LDAP integrada ao portal. | Geral |
| **Central de RH** | Consultas administrativas e suporte ao colaborador. | Funcionário |
| **Gestão de Perfil** | Controle granular de acesso baseado em papéis (RBAC). | Sistema |

### 1.3. Ecossistema de Integrações Internas

*Fluxos de sincronismo e comunicação desenvolvidos pela equipe.*

| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **GrupoA (Manager)**| [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Sincronismo LXP -> RM (Portal) | Marcelo |
| **GrupoA (Avalia)** | .NET Framework | Integração antiga Avalia -> RM | Marcelo |
| **Biblioteca Dig.** | `Minha Biblioteca` (PHP) | Sincronismo de usuários RM -> Grupo A | Marcelo |
| **Módulo Valorizza**| Integração (Portal) | Integração Valorizza (Reside no Portal) | Marcelo |
| **Sincronismo AD** | Integração RM -> AD | Manutenção de usuários no Active Directory | Marcelo |
| **Custom RM (Low)** | Fórmulas Visuais / SQL | Lógica interna e gatilhos do ERP | Marcelo |
| **Processos BPM** | Fluig (Processos) | Fluxos de trabalho customizados (Ex: SAE, Compras) | Theo |
| **Dashboards BI** | Power BI (Dashboards) | Painéis estratégicos desenvolvidos internamente | Thiago |

### 1.3. Bibliotecas, APIs e Helpers (Infraestrutura de Código)
| Helper | Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **API TOTVS** | [`lib-api-totvs`](https://github.com/uniarpdev/lib-api-totvs) | Cliente de integração com APIs TOTVS | Marcelo |
| **API LDAP** | [`lib-api-ldap`](https://github.com/uniarpdev/lib-api-ldap) | Biblioteca de comunicação com servidor LDAP | Marcelo |
| **API Grupo A** | [`lib-api-grupoa`](https://github.com/uniarpdev/lib-api-grupoa) | Conector para APIs GrupoA-MaisCampus | Marcelo |
| **API Valorizza** | [`lib-api-valorizza`](https://github.com/uniarpdev/lib-api-valorizza) | Conector para APIs da Valorizza | Marcelo |
| **Dotnet Utils** | [`lib-dotnet-utils`](https://github.com/uniarpdev/lib-dotnet-utils) | Helpers gerais para projetos .NET C# | Marcelo |
| **Scripts & Tasks** | [`uniarpTasks`](https://github.com/uniarpdev/uniarpTasks) | Automações e tarefas agendadas | Marcelo |

---

## 🛠️ PARTE 2: SUSTENTAÇÃO DE SISTEMAS DE TERCEIROS (Suporte)
*Plataformas adquiridas onde a equipe realiza parametrização, suporte e garantia de disponibilidade.*

### 2.1. Núcleo ERP (TOTVS RM) - Supervisão Geral: **Rolff**
| Módulo / Produto | Tecnologia | Descrição | Analista Resp. |
| :--- | :--- | :--- | :--- |
| **Educacional** | RM Classis Net | Gestão acadêmica e enturmação | Rolff |
| **Financeiro** | RM Fluxus | Gestão de contas a pagar/receber e caixa | Maria |
| **Contábil / Fiscal**| RM Saldus / Liber | Escrituração, impostos e contabilidade | Maria |
| **Folha / RH** | RM Labore / Vitae | Gestão de pessoas e pagamentos | Dionathan |
| **Ponto Eletrônico** | RM Chronus | Gestão de jornada de trabalho | Dionathan |
| **Estoque / Compras** | RM Nucleus | Suprimentos e faturamento | Maria |
| **Biblioteca** | RM Biblios | Gestão de acervo físico | David |

### 2.2. Plataformas Satélites e Serviços
| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Portal Educacional**| Totvs (RM) | Interface nativa RM (Alunos/Prof) | Rolff |
| **Minha Uniarp (App)**| Totvs (Mobile) | Aplicativo mobile acadêmico | Rolff |
| **Meu RH (App)** | Totvs (Mobile) | Gestão de comunicação com colaboradores | Rolff |
| **Meu RH (Web)** | Totvs (Web) | Portal web para colaboradores | Rolff |
| **Suricato** | Telemática | Gestão de segurança física e acesso | Dionathan |
| **Fluig (Plataforma)**| Totvs | Ambiente de BPM e Portais | Theo |
| **Plataforma LXP** | +Campus/GrupoA | Ambiente Virtual de Aprendizagem | A definir |
| **GPA** | +Campus/GrupoA | Gestão de projetos e atividades acadêmicas | A definir |
| **NPJ** | +Campus/GrupoA | Núcleo de Práticas Jurídicas | A definir |
| **Avalia** | +Campus/GrupoA | Plataforma de avaliações e provas | A definir |
| **Assinatura Digit.**| TAE Totvs Assinatura | Assinatura eletrônica de documentos | A definir |
| **Atendimento Whats** | WorkChat | Automação via WhatsApp | A definir |
| **Gestão Carreira** | Valorizza | Plataforma de gestão de carreira | A definir |
| **CRM / Marketing** | Rubeus | Gestão de relacionamento e captação | David |
| **Ponto (Kairos)** | Kairos (Dimep) | Coleta de registros de ponto | Dionathan |
| **GED / Diplomas** | DocXpress/Diplomax| Digitalização e gestão de diplomas | Eduardo |
| **Gestão de TI** | `GLPI` | Gerenciamento de chamados e ativos | Marcelo |
| **Office 365** | Microsoft | Power Automate e ferramentas Office | Dionathan |
| **Impressão** | `SafePrint` | Gestão de cotas de impressão | Kamile |

---
*Nota: Este catálogo reflete o levantamento oficial de 2025 consolidado com o planejamento de 2026.*
