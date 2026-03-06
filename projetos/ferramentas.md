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
| **Portais Diversos** | PHP / Web | SEDEPEX, Egresso, Jogos, Acervo e LGPD | Andre |
| **Monitoria** | `Bubble.io` | Gestão de agendamento de monitorias (No-Code) | Thiago |
| **Gestão de Frotas** | [`app-gestao-frotas`](https://github.com/uniarpdev/app-gestao-frotas) | Controle de veículos (Bubble/Interno) | Thiago |

### 1.2. Bibliotecas, APIs e Helpers (Infraestrutura de Código)
| Helper | Repositório | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **API TOTVS** | [`lib-api-totvs`](https://github.com/uniarpdev/lib-api-totvs) | Cliente de integração com APIs TOTVS | Marcelo |
| **API LDAP** | [`lib-api-ldap`](https://github.com/uniarpdev/lib-api-ldap) | Biblioteca de comunicação com servidor LDAP | Marcelo |
| **API Grupo A** | [`lib-api-grupoa`](https://github.com/uniarpdev/lib-api-grupoa) | Conector para APIs GrupoA-MaisCampus | Marcelo |
| **API Valorizza** | [`lib-api-valorizza`](https://github.com/uniarpdev/lib-api-valorizza) | Conector para APIs da Valorizza | Marcelo |
| **Dotnet Utils** | [`lib-dotnet-utils`](https://github.com/uniarpdev/lib-dotnet-utils) | Helpers gerais para projetos .NET C# | Marcelo |
| **Scripts & Tasks** | [`uniarpTasks`](https://github.com/uniarpdev/uniarpTasks) | Automações e tarefas agendadas | Marcelo |

### 1.3. Customizações e Integrações Internas
| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Integrador Acad.** | [`app-academico`](https://github.com/uniarpdev/app-academico) | Automação de processos RM (Console) | Marcelo |
| **Notas (Manager)** | [`app-portal-mvc`](https://github.com/uniarpdev/app-portal-mvc) | Sincronismo LXP -> RM (Portal) | Marcelo |
| **Notas (Avalia)** | .NET Framework | Integração antiga Avalia -> RM | Marcelo |
| **Biblioteca Dig.** | `Minha Biblioteca` (PHP) | Sincronismo de usuários RM -> Grupo A | Marcelo |
| **Módulo Valorizza**| Integração (Portal) | Integração Valorizza (Reside no Portal) | Marcelo |
| **Sincronismo AD** | Integração RM -> AD | Manutenção de usuários no Active Directory | Marcelo |
| **Custom RM (Low)** | Fórmulas Visuais / SQL | Lógica interna e gatilhos do ERP | Marcelo |
| **Processos BPM** | Fluig (Processos) | Fluxos de trabalho customizados (Ex: SAE, Compras) | Theo |
| **Dashboards BI** | Power BI (Dashboards) | Painéis estratégicos desenvolvidos internamente | Marcelo/Thiago |

---

## 🛠️ PARTE 2: SUSTENTAÇÃO DE SISTEMAS DE TERCEIROS (Suporte)
*Plataformas adquiridas onde a equipe realiza parametrização, suporte e garantia de disponibilidade.*

### 2.1. Núcleo ERP (TOTVS RM) - Supervisão Geral: **Rolff**
| Módulo / Produto | Tecnologia | Descrição | Analista Resp. |
| :--- | :--- | :--- | :--- |
| **Educacional** | RM Classis Net | Gestão acadêmica e enturmação | A definir |
| **Financeiro** | RM Fluxus | Gestão de contas a pagar/receber e caixa | A definir |
| **Contábil / Fiscal**| RM Saldus / Liber | Escrituração, impostos e contabilidade | A definir |
| **Folha / RH** | RM Labore / Vitae | Gestão de pessoas e pagamentos | A definir |
| **Ponto Eletrônico** | RM Chronus | Gestão de jornada de trabalho | A definir |
| **Estoque / Compras** | RM Nucleus | Suprimentos e faturamento | A definir |
| **Biblioteca** | RM Biblios | Gestão de acervo físico | A definir |
| **Segurança / Saúde** | RM Agilis / Bonum | Atendimento e gestão patrimonial | A definir |

### 2.2. Plataformas Satélites e Serviços
| Produto | Tecnologia | Descrição | Ponto Focal |
| :--- | :--- | :--- | :--- |
| **Portal Educacional**| Totvs (RM) | Interface nativa RM (Alunos/Prof) | Rolff |
| **Minha Uniarp (App)**| Totvs (Mobile) | Aplicativo mobile acadêmico | Rolff |
| **Meu RH (App)** | Totvs (Mobile) | Gestão de comunicação com colaboradores | Rolff |
| **Suricato** | Telemática | Gestão de segurança física e acesso | Marcelo |
| **Fluig (Plataforma)**| Totvs | Ambiente de BPM e Portais | Theo |
| **Plataforma LXP** | Grupo A | Ambiente Virtual de Aprendizagem | Marcelo |
| **Módulo Orbita** | Integração RM | Geração de matrículas (Orbita -> RM) | A definir |
| **Assinatura Digit.**| Sign (Totvs) | Assinatura eletrônica de documentos | A definir |
| **Atendimento Whats** | WorkChat | Automação via WhatsApp | A definir |
| **Gestão Carreira** | WorkAlove | Plataforma de gestão de carreira | A definir |
| **Site Institucional** | WordPress | Site público uniarp.edu.br | Andre |
| **CRM / Marketing** | Rubeus | Gestão de relacionamento e captação | A definir |
| **Ponto (Kairos)** | Kairos (Dimep) | Coleta de registros de ponto | A definir |
| **GED / Diplomas** | DocXpress/Diplomax| Digitalização e gestão de diplomas | A definir |
| **Gestão de TI** | `GLPI` | Gerenciamento de chamados e ativos | Marcelo |
| **Office 365** | Microsoft | Power Automate e ferramentas Office | Dionathan |
| **Impressão** | `SafePrint` | Gestão de cotas de impressão | Dionathan |

---
*Nota: Este catálogo reflete o levantamento oficial de 2025 consolidado com o planejamento de 2026.*
