# 📑 Product Requirements Document (PRD)

**Produto:** Plataforma “ArchAI” – Architecture as Code + Agentes de IA Corporativa
**Versão:** Draft 0.1
**Data:** Outubro/2025

---

## 1. Visão Geral

A ArchAI é uma plataforma que combina **IA generativa (LLMs)** com a disciplina de **arquitetura corporativa** em frameworks reconhecidos (TOGAF, eTOM, TAM – TM Forum).
Objetivo: permitir que arquitetos, gestores de TI e executivos criem, mantenham e governem arquiteturas **como código (Architecture as Code)**, com suporte a **agentes inteligentes** para geração, validação e evolução contínua dos modelos.

Problema a resolver:

* Documentação arquitetural fragmentada, desatualizada e de difícil governança.
* Falta de automação no ciclo de arquitetura corporativa.
* Dificuldade em alinhar frameworks globais (TOGAF, TM Forum) com ferramentas práticas do dia a dia (LeanIX, ArchiMate, C4 Model).

---

## 2. Objetivos

* **Estratégicos:**

  * Modernizar a prática de arquitetura corporativa com IA.
  * Reduzir custos de governança e aumentar a velocidade de atualização.
  * Garantir compliance regulatório e aderência a frameworks.

* **Táticos:**

  * Automatizar geração de diagramas ArchiMate/C4.
  * Orquestrar repositórios de arquitetura (LeanIX, Ardoq, repos Git).
  * Criar assistentes virtuais (agents) que respondem sobre a arquitetura em linguagem natural.

---

## 3. Stakeholders

* **Primários:** Arquitetos corporativos, Enterprise Architecture Offices (EAOs).
* **Secundários:** Executivos C-Level (CIO, CTO, CFO), times de inovação e compliance.
* **Parceiros:** Fornecedores de SaaS de arquitetura (LeanIX, Ardoq, Bizzdesign).

---

## 4. Escopo

* **Incluído:**

  * Geração de modelos TOGAF, eTOM e TAM automatizados.
  * Conector nativo para LeanIX, ArchiMate e modelos C4.
  * Agents para governança e respostas em tempo real (RAG + LLM).
  * Exportação Architecture as Code em YAML/JSON.

* **Excluído (versão inicial):**

  * Integração com todas as ferramentas de ITSM/DevOps.
  * Suporte completo a todas as variantes do TM Forum (TAM detalhado em micro-níveis).

---

## 5. Casos de Uso / User Stories

* **Como arquiteto**, quero gerar um modelo TOGAF de baseline architecture automaticamente a partir de entrevistas textuais, para reduzir o tempo inicial de modelagem.
* **Como gestor**, quero validar gaps com frameworks TM Forum em tempo real, para identificar áreas não cobertas.
* **Como executivo**, quero receber dashboards e KPIs traduzidos em linguagem de negócios, para apoiar decisões.

---

## 6. Requisitos Funcionais

* R1: Importar e exportar modelos em formatos compatíveis (ArchiMate XML, LeanIX API, C4 DSL).
* R2: Gerar diagramas automaticamente com base em prompts em linguagem natural.
* R3: Suporte a consultas em linguagem natural sobre a arquitetura.
* R4: Versionamento e governança com repositório Git (Architecture as Code).

---

## 7. Requisitos Não Funcionais

* Segurança: suporte a RBAC e SSO corporativo.
* Performance: resposta de agentes em <3s em consultas padrão.
* Compliance: aderência a GDPR/LGPD e frameworks de EA.
* Observabilidade: logs detalhados e métricas de uso.

---

## 8. Integrações

* **Ferramentas de EA:** LeanIX, Ardoq, Bizzdesign.
* **Modelagem:** ArchiMate, C4 Model.
* **Infra:** GitHub/GitLab (Arquitetura como código).
* **AI/LLM:** OpenAI GPT-5, Anthropic Claude, LangChain.

---

## 9. KPIs & Métricas

* % de atualização automática de modelos.
* Tempo médio de geração de arquitetura baseline.
* Nível de aderência aos frameworks (TOGAF, eTOM, TAM).
* Engajamento dos usuários (consultas/semana).

---

## 10. Roadmap Macro

* **Fase 1 (MVP, 6 meses):** Conector LeanIX + Geração ArchiMate via prompt.
* **Fase 2 (12 meses):** Agents com RAG integrado a repositório Git.
* **Fase 3 (18 meses):** Validação automática contra eTOM/TAM.
* **Fase 4 (24 meses):** Dashboards executivos + marketplace de agentes de arquitetura.

---

## 11. Riscos e Dependências

* Dependência de APIs de terceiros (LeanIX, OpenAI).
* Acurácia dos LLMs em contextos técnicos específicos.
* Resistência cultural das áreas de arquitetura tradicional.
* Risco de lock-in em fornecedores de IA.
