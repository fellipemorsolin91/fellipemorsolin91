# 👋 Fellipe Oliveira Morsolin

**Database Solutions Architect | 13+ anos em Oracle, PostgreSQL, MongoDB & ClickHouse**

🎯 Especialista em **performance tuning**, **alta disponibilidade** e **automação DBA**  
🏢 Nexxera • Florianópolis, SC, Brazil

---

## 🔧 Stack Principal

**Databases:**  
`Oracle` `PostgreSQL` `MongoDB` `ClickHouse` `MySQL` `MariaDB` `SQL Server`

**Especialidades:**  
Performance Tuning • AWR Analysis • Query Optimization • High Availability • Sharding & Replication • Automation

**DevOps & Tools:**  
`Python` `Bash` `PowerShell` `Git` `Zabbix` `Docker` `GitHub Copilot`

---

## 💼 Foco Atual

- 🚀 **Pattern-Based Architecture** - Zero invenção, 100% baseado em ambientes reais
- 🧠 **Knowledge System** - ChromaDB + 16 AI-Powered Agent Personas
- 📊 **Database Analytics** - Integração Zabbix + métricas de performance
- 🤖 **DBA Automation** - Workflows inteligentes com GitHub Copilot

---

## 🛠️ Experiência Técnica

**Oracle** → RAC, Data Guard, ASM, AWR Analysis, PL/SQL  
**PostgreSQL** → MVCC, Replication, Extensions, VACUUM tuning  
**MongoDB** → Sharding, Replica Sets, Aggregation Framework  
**ClickHouse** → MergeTree, Compression, PREWHERE, Materialized Views

---

## 🚀 Projetos Destacados

### 🗄️ **DBA-WORKSPACE** - Multi-Platform Database Operations Framework
Ambiente de trabalho inteligente com 16 personas especializadas AI + ChromaDB knowledge engine

**Stack:** `Python` `GitHub Copilot` `ChromaDB` `Pattern-Based Architecture`  
**Cobertura:** Oracle, PostgreSQL, MongoDB, ClickHouse, MySQL, MariaDB, SQL Server

🔗 **[Ver Repositório](https://github.com/fellipemorsolin91/DBA-WORKSPACE)**

**Features:**
- Sistema de learnings persistente cross-session com vector embeddings
- Detecção automática de contexto e mudança de persona
- Padrões extraídos de ambientes reais (zero invenção)
- Workflows com aprovação explícita para operações destrutivas

---

### 🔐 **Automated Multi-Database Audit & Compliance System**
Sistema enterprise de auditoria automatizada para governança de acesso em ambiente multi-database

**Desafio:**  
Geração manual de relatórios de compliance (LGPD, auditoria interna) exigia **4-6 horas** de trabalho manual por ciclo:
- Conexão individual em 30+ instâncias de bancos diferentes
- Extração manual de usuários, roles, grants e permissões
- Consolidação em planilhas separadas por SGBD
- Formatação e envio para áreas de segurança/compliance

**Solução:**  
Automação completa end-to-end com Python + drivers nativos multi-SGBD

**Stack:** `Python` `Oracle` `PostgreSQL` `MongoDB` `MySQL` `CSV Automation`  
**Ambientes:** 30+ instâncias em produção (5 MySQL, 15 PostgreSQL, 10 Oracle, 4 MongoDB)

**Resultados:**
- ⏱️ **Tempo:** 4-6 horas → **15 minutos** (redução de **95%**)
- 📊 **Precisão:** 100% (eliminação de erros humanos em consolidação)
- 🔄 **Frequência:** Mensal → On-demand (sob demanda imediata)
- 📈 **Escalabilidade:** Suporta novos SGBDs sem refatoração

**Impacto:**
- Compliance proativa com relatórios atualizados sempre disponíveis
- Redução de riscos de auditoria (dados sempre atualizados)
- Liberação de 4-6h/mês de trabalho manual para atividades estratégicas

---

### 🔍 **Real-Time User Existence Checker Across Multiple Databases**
Ferramenta de análise instantânea para verificação de usuários/schemas em infraestrutura multi-database

**Desafio:**  
Atendimento de chamados (GA, GDV, GMA) exigia verificação manual de existência de usuários:
- **Processo anterior:** 30-45 minutos por análise
  - Consultar documentação de hosts (5-10 min)
  - Conectar manualmente em cada instância (15-20 min)
  - Executar queries específicas por SGBD (5-10 min)
  - Consolidar resultados em texto/email (5 min)
- **Frequência:** 15-20 solicitações/mês = **8-15 horas/mês**

**Solução:**  
Script Python orquestrador com execução paralela em todos os bancos

**Stack:** `Python` `Multi-Threading` `Oracle cx_Oracle` `psycopg2` `pymongo` `MySQL Connector`  
**Cobertura:** 30+ servers (PRD + QA + DEV + TST)

**Resultados:**
- ⚡ **Tempo:** 30-45 min → **<2 minutos** (redução de **95%**)
- 📋 **Output:** Relatório consolidado automático (txt) com status por servidor
- 🎯 **Precisão:** 100% - varre TODAS as instâncias sem exceção
- 🔄 **Reusabilidade:** Único comando para qualquer usuário

**Exemplo de uso:**
```bash
python user_checker.py zabbix
# Output: Relatório em <2 min com status em 30+ servidores
```

**Impacto:**
- **8-15 horas/mês** economizadas em análises manuais
- SLA de atendimento reduzido drasticamente
- Suporte a decisões rápidas (remover acessos, validar deployments)

---

### ⚙️ **Oracle Roles & Access Automation Framework**
Framework de padronização e provisionamento automático de acessos Oracle com geração dinâmica de grants/synonyms

**Desafio:**  
Criação manual de roles e acessos em schemas Oracle apresentava riscos:
- **Processo anterior:** 20-30 minutos por schema
  - Definição manual de grants objeto por objeto (10-15 min)
  - Criação manual de synonyms no schema de aplicação (5-10 min)
  - Testes de validação (5 min)
  - Risco de esquecimento de objetos (erros em produção)
- **Inconsistência:** Padrões diferentes entre schemas/ambientes
- **Frequência:** 3-5 novos schemas/mês = **2-3 horas/mês** + retrabalho

**Solução:**  
Sistema centralizado com templates PL/SQL + automação Shell Script

**Stack:** `Oracle PL/SQL` `Shell Script` `Automation Framework` `Template-Based`  
**Ambientes:** Oracle 11g + 19c (INT)

**Arquitetura:**
- Roles padronizadas: `ROLE_<SCHEMA>_R` (read-only), `ROLE_<SCHEMA>_RW` (read-write), `ROLE_<SCHEMA>_APP` (application)
- Geração automática de grants para TODOS os objetos existentes
- Criação automática de synonyms no schema de aplicação
- HOW-TO documentado para replicação

**Resultados:**
- ⏱️ **Tempo:** 20-30 min → **<5 minutos** (redução de **83%**)
- 🎯 **Erros:** 100% eliminados (nenhum objeto esquecido)
- 📐 **Padronização:** 100% consistência entre schemas/ambientes
- 🔄 **Reusabilidade:** Template aplicável a qualquer novo schema

**Exemplo de deployment:**
```sql
@create_roles_and_grants.sql SCHEMA_NAME
-- Output: Roles criadas + Grants aplicados + Synonyms gerados em <5 min
```

**Impacto:**
- **2-3 horas/mês** economizadas + eliminação de retrabalho
- Zero incidentes de "acesso não funciona" pós-deployment
- Onboarding de novos schemas 83% mais rápido
- Compliance: auditoria facilitada (padrões documentados)

---

## 📊 Resumo de Impacto

**Economia total mensal:** ~**15-24 horas** em automações  
**Redução de erros:** **100%** em processos automatizados  
**ROI:** Frameworks reutilizáveis em múltiplos projetos  
**Escalabilidade:** Soluções suportam crescimento sem refatoração

---

## 📫 Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fellipe-oliveira-morsolin-69497a2a/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:fellipemorsolin@gmail.com)

---

*"Medir antes de otimizar. Entender antes de mudar. Testar antes de aprovar."*
