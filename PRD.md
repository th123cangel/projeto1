# 📑 Product Requirements Document (PRD)

**Produto:** Plataforma “ArchAI” – Architecture as Code + Agentes de IA Corporativa  
**Versão:** Draft 0.2 (revisado)  
**Data:** Outubro/2025  
**Autor:** Arquitetura & IA Lab

---

## Sumário Executivo

A ArchAI é uma plataforma que combina **IA generativa (LLMs)** com a disciplina de **arquitetura corporativa** em frameworks reconhecidos (TOGAF, eTOM, TAM – TM Forum). Seu objetivo é permitir que arquitetos, gestores de TI e executivos criem, mantenham e governem arquiteturas **como código (Architecture as Code)**, apoiados por **agentes inteligentes** que aceleram a geração, validação e evolução contínua dos modelos.

### Principais problemas resolvidos

* Documentação arquitetural fragmentada, desatualizada e de difícil governança.
* Baixa automação no ciclo de arquitetura corporativa e nas integrações com ferramentas de mercado.
* Dificuldade em alinhar frameworks globais (TOGAF, TM Forum) com ferramentas práticas do dia a dia (LeanIX, ArchiMate, C4 Model).

### Proposta de valor

* **Velocidade:** geração assistida de modelos e artefatos em minutos, não semanas.
* **Confiabilidade:** governança contínua, versionamento como código e validação automática com frameworks.
* **Inteligência aplicada:** agentes conversacionais com RAG respondendo em linguagem natural, orientando decisões e auditorias.

---

## Tabela de Conteúdo

1. [Objetivos](#objetivos)
2. [Personas e Stakeholders](#personas-e-stakeholders)
3. [Escopo](#escopo)
4. [Casos de Uso / User Stories](#casos-de-uso--user-stories)
5. [Requisitos Funcionais](#requisitos-funcionais)
6. [Requisitos Não Funcionais](#requisitos-não-funcionais)
7. [Integrações](#integrações)
8. [KPIs & Métricas](#kpis--métricas)
9. [Roadmap Macro](#roadmap-macro)
10. [Riscos, Dependências e Mitigações](#riscos-dependências-e-mitigações)
11. [Suposições e Questões em Aberto](#suposições-e-questões-em-aberto)

---

## Objetivos

**Estratégicos**

* Modernizar a prática de arquitetura corporativa com IA, reduzindo o tempo para documentar e alinhar arquiteturas.
* Garantir compliance regulatório e aderência a frameworks globalmente reconhecidos.
* Aumentar a visibilidade executiva sobre investimentos e riscos de arquitetura.

**Táticos**

* Automatizar geração e atualização de diagramas ArchiMate/C4 em repositórios Git.
* Orquestrar repositórios de arquitetura (LeanIX, Ardoq) com pipelines de validação contínua.
* Disponibilizar assistentes virtuais (agents) que respondem sobre a arquitetura em linguagem natural.

**Métricas de Sucesso (Leading Indicators)**

* Redução de 60% no tempo médio de geração de baseline architecture em 6 meses.
* Aumento de 40% no número de decisões suportadas por evidências arquiteturais.
* Net Promoter Score (NPS) ≥ 45 entre arquitetos corporativos após o MVP.

---

## Personas e Stakeholders

* **Arquiteto Corporativo (persona primária):** responsável por modelar e governar a arquitetura; precisa de automação, rastreabilidade e consistência de frameworks.
* **Gestor de Portfólio de TI:** busca visibilidade sobre iniciativas, dependências e impactos de mudanças.
* **Executivo C-Level (CIO/CTO/CFO):** necessita de insights traduzidos em métricas de negócio e relatórios para auditorias.
* **Equipe de Compliance e Risco:** garante aderência a políticas internas e regulações (LGPD, GDPR).
* **Parceiros SaaS:** fornecedores de EA (LeanIX, Ardoq, Bizzdesign) que possibilitam integrações e co- inovação.

Stakeholders secundários incluem times de inovação, squads de modernização e consultorias especializadas em arquitetura empresarial.

---

## Escopo

**Incluído**

* Geração automatizada de modelos TOGAF, eTOM e TAM a partir de prompts guiados e documentos base.
* Conectores nativos para LeanIX, ArchiMate e modelos C4 com sincronização bidirecional.
* Agents de governança com RAG para responder questões em tempo real, inclusive auditoria básica.
* Exportação Architecture as Code em YAML/JSON e versionamento Git com pipelines de validação.

**Excluído (versão inicial)**

* Integração com todas as ferramentas de ITSM/DevOps ou CMDBs legadas.
* Suporte detalhado a todas as variantes do TM Forum (micro-níveis do TAM).
* Automação de processos de FinOps ou gestão de custos multicloud.

**Limitações Conhecidas**

* Dependência de dados estruturados fornecidos pelos clientes para gerar modelos de alta fidelidade.
* Disponibilidade inicial apenas em português e inglês (localização adicional considerada fase 3).

---

## Casos de Uso / User Stories

1. **Como arquiteto**, quero gerar um modelo TOGAF de baseline architecture automaticamente a partir de entrevistas textuais, para reduzir o tempo inicial de modelagem.
2. **Como gestor**, quero validar gaps com frameworks TM Forum em tempo real, para identificar áreas não cobertas e planejar ações corretivas.
3. **Como executivo**, quero receber dashboards e KPIs traduzidos em linguagem de negócios, para apoiar decisões e apresentações ao board.
4. **Como analista de compliance**, quero auditar mudanças arquiteturais e rastrear decisões relevantes em um log único.
5. **Como líder de inovação**, quero experimentar variações de modelos de referência (blueprints) e comparar cenários.

Cada história terá critérios de aceite documentados no backlog tático (fora do escopo deste PRD) com foco em evidências mensuráveis.

---

## Requisitos Funcionais

* **R1 – Orquestração de Modelos:** importar e exportar modelos em formatos compatíveis (ArchiMate XML, LeanIX API, C4 DSL) com versionamento automático.
* **R2 – Geração Assistida:** gerar diagramas automaticamente com base em prompts em linguagem natural, templates e reutilização de componentes.
* **R3 – Interação Conversacional:** oferecer consultas em linguagem natural com agentes especializados e memória contextual.
* **R4 – Governance as Code:** versionar políticas, catálogos e decisões arquiteturais em repositório Git com revisão/aprovação (pull requests).
* **R5 – Analytics & Dashboards:** disponibilizar painéis pré-configurados e exportação de KPIs em formatos abertos (CSV, PowerBI connector).

---

## Requisitos Não Funcionais

* **Segurança:** suporte a RBAC, SSO corporativo (OIDC/SAML) e trilhas de auditoria.
* **Performance:** resposta média dos agentes <3s em consultas padrão com capacidade de escala horizontal.
* **Confiabilidade:** disponibilidade alvo de 99,5% para componentes críticos e política de backup diário.
* **Compliance:** aderência a GDPR/LGPD, padrões de retenção de dados e certificações SOC2 tipo II na fase 2.
* **Observabilidade:** logs detalhados, métricas de uso e alertas proativos integrados a ferramentas de APM.

---

## Integrações

* **Ferramentas de EA:** LeanIX, Ardoq, Bizzdesign.
* **Modelagem:** ArchiMate, C4 Model, BPMN (exploração fase 2).
* **Infraestrutura:** GitHub/GitLab (arquitetura como código), armazenamento de blobs (S3/Azure Blob) para anexos.
* **AI/LLM:** OpenAI GPT-5, Anthropic Claude, LangChain, com opção BYO-LLM para clientes regulados.

---

## KPIs & Métricas

* **Eficiência Operacional:** % de atualização automática de modelos vs. atualizações manuais.
* **Time-to-Value:** tempo médio de geração de arquitetura baseline e de aprovação de mudanças.
* **Aderência a Frameworks:** cobertura (%) dos domínios TOGAF, eTOM, TAM monitorados automaticamente.
* **Engajamento:** consultas por semana por persona, taxa de adoção de agentes e NPS trimestral.

Os KPIs serão revisados trimestralmente em conjunto com o escritório de arquitetura e times de produto.

---

## Roadmap Macro

* **Fase 1 (MVP – 6 meses):** Conector LeanIX, geração ArchiMate via prompt, dashboard operacional básico.
* **Fase 2 (12 meses):** Agents com RAG integrado a repositório Git, BYO-LLM e auditoria automatizada.
* **Fase 3 (18 meses):** Validação automática contra eTOM/TAM, suporte a BPMN e expansão de idiomas.
* **Fase 4 (24 meses):** Dashboards executivos avançados, marketplace de agentes de arquitetura e integrações adicionais (ServiceNow, Jira Align).

---

## Riscos, Dependências e Mitigações

* **Dependência de APIs de terceiros (LeanIX, OpenAI):** estabelecer acordos de nível de serviço e opções alternativas (ex.: API GraphQL interna, modelos open source em nuvem privativa).
* **Acurácia dos LLMs em contextos técnicos específicos:** montar equipe de curadoria de conhecimento e implementar feedback loop humano.
* **Resistência cultural das áreas de arquitetura tradicional:** programa de change management com workshops e champions.
* **Risco de lock-in em fornecedores de IA:** arquitetura modular com camadas de abstração para troca de provedores.
* **Segurança e confidencialidade:** governança de dados sensíveis e criptografia ponta a ponta para ativos de arquitetura.

---

## Suposições e Questões em Aberto

* Clientes possuem inventário mínimo de ativos e processos para alimentar o motor de geração.
* Disponibilidade de budget para licenciamento de LLMs premium durante o MVP.
* Questões em aberto: modelo de precificação (por assento vs. por consumo), estratégia de parcerias com consultorias de EA, roadmap de certificações adicionais.

> Documento sujeito a revisões trimestrais conforme evolução das descobertas de produto e feedback dos stakeholders.
