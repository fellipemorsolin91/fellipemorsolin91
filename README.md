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
**MySQL** → InnoDB, Replication, Performance Schema, Query Optimization  
**MariaDB** → Galera Cluster, ColumnStore, MaxScale, XtraDB  
**SQL Server** → Always On, Query Store, T-SQL, Index Tuning

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
Geração manual de relatórios de compliance (LGPD, auditoria interna) exigia **até 1 semana (40h+)** de trabalho por ciclo:
- Conexão individual em 39 instâncias de bancos diferentes
- Extração manual de usuários, roles, grants e permissões
- Consolidação em planilhas separadas por SGBD
- Formatação e envio para áreas de segurança/compliance
- Alto risco de erro humano e omissões
- Processo não repetível nem auditável de forma confiável

**Solução:**  
Automação completa end-to-end com detection automática de SGBDs e execução de queries específicas por tecnologia

**Stack:** `Python` `Oracle` `PostgreSQL` `MongoDB` `MySQL` `MariaDB` `CSV Automation`  
**Ambientes:** 39 instâncias em produção (5 MySQL, 22 PostgreSQL, 4 Oracle, 4 MariaDB, 4 MongoDB)

**Resultados:**
- ⏱️ **Tempo:** 1 semana (40h+) → **20 minutos** (redução de **98%**)
- 📊 **Precisão:** Risco de erro alto → Praticamente zero
- 🔄 **Frequência:** Trimestral/semestral → Diária/semanal sob demanda
- 📈 **Escalabilidade:** Estrutura expansível para novos ambientes

**Impacto:**
- Melhoria na governança e conformidade de acessos
- Geração de relatórios auditáveis com histórico automatizado
- Liberação de tempo operacional para tarefas estratégicas
- Notificação automática por e-mail integrado

---

### 🔍 **Real-Time User Existence Checker Across Multiple Databases**
Ferramenta de análise instantânea para verificação de usuários/schemas em infraestrutura multi-database

**Desafio:**  
Atendimento de chamados (GA, GDV, GMA, INF) e demandas via Hangouts exigia verificação manual de existência de usuários:
- **Processo anterior:** 20 a 60 minutos por análise
  - Conexões diretas em cada instância de forma sequencial
  - Execução de queries específicas por SGBD (Oracle, PostgreSQL, MySQL, MariaDB, MongoDB)
  - Dificuldade em detectar inconsistências rapidamente
  - Alto risco de erro humano e omissão de instâncias
- **Processo não auditável nem padronizado**

**Solução:**  
Módulo automatizado Python com execução paralela e geração de relatórios padronizados

**Stack:** `Python` `Multi-Threading` `Oracle cx_Oracle` `psycopg2` `pymongo` `MySQL Connector` `MariaDB`  
**Cobertura:** Múltiplas instâncias heterogêneas (PRD + QA + DEV + TST)

**Resultados:**
- ⚡ **Tempo:** 20-60 min → **~5 segundos** (redução de **~99,8%**)
- 📋 **Output:** Arquivo .txt com resultados consolidados automático
- 🎯 **Precisão:** Risco alto → Praticamente zero
- 🔄 **Frequência:** Esporádica → Diária ou sob demanda

**Exemplo de uso:**
```bash
python user_checker.py <username>
# Output: Relatório em ~5 segundos com status em todas as instâncias
```

**Impacto:**
- Validação imediata de usuários e schemas em múltiplos SGBDs
- Aplicação direta em chamados GA, GDV, GMA, INF e demandas via Hangouts
- Processo auditável, reproduzível e facilmente expansível
- Exemplo real: GDV-14373

---

### ⚙️ **Oracle Roles & Access Automation Framework**
Framework de padronização e provisionamento automático de acessos Oracle com triggers e geração dinâmica de grants/synonyms

**Desafio:**  
Criação manual de roles e acessos em schemas Oracle apresentava riscos operacionais e de governança:
- Grants diretos sobre tabelas/sequences geravam **locks DDL** em alta concorrência (ambiente MERCANTIL)
- Risco de esquecimento de objetos em deploys (erros em produção)
- Inconsistência de padrões entre schemas e ambientes (TST, QAI, QAE, PRD)
- Processo manual de concessão objeto por objeto
- Dependência de intervenção manual pós-deploy
- Pipelines de CI/CD não previsíveis

**Solução:**  
Arquitetura baseada em roles padronizadas + triggers automáticas que monitoram criação de objetos

**Stack:** `Oracle PL/SQL` `Triggers` `Oracle Scheduler Jobs` `Shell Script` `Template-Based`  
**Ambientes:** Oracle 11g + 19c (INT)

**Arquitetura:**
- **Roles padronizadas:** `ROLE_<SCHEMA>_R` (read-only), `ROLE_<SCHEMA>_RW` (read-write), `ROLE_<SCHEMA>_APP` (application)
- **Triggers automáticas:** Monitoram criação de tabelas, views, materialized views, sequences, packages, functions, procedures
- **Jobs Oracle Scheduler:** Executam grants e synonyms 5 segundos após criação do objeto, depois se autodestroem
- **Automação completa:** Schema de aplicação mantém acesso atualizado sem intervenção manual

**Ganhos técnicos e operacionais:**

**1. Eliminação de bloqueios DDL:**
- Permissões aplicadas apenas às roles (não às estruturas físicas)
- Zero locks em objetos de dados (eliminação completa de contenções)

**2. Controle centralizado:**
- Todos os privilégios nas roles (revogações/restaurações imediatas)
- Backup completo permite restauração a qualquer momento

**3. Redução de erro humano:**
- Toda nova estrutura recebe automaticamente privilégios e synonyms corretos
- Zero necessidade de ajustes manuais pós-deploy

**4. Estabilidade CI/CD:**
- Pipelines previsíveis e reprodutíveis
- Schema de aplicação com acesso completo após cada deploy

**5. Governança e escalabilidade:**
- Atribuir usuário a role = único passo necessário para acesso
- Facilita auditorias e padroniza entre ambientes

**Exemplo de deployment:**
```sql
@create_roles_and_grants.sql SCHEMA_NAME
-- Output: Roles criadas + Grants automáticos via triggers + Synonyms gerados
```

**Resultado real (antes/depois):**
- **Antes:** 60 grants diretos em usuários na tabela PAG_LOTE
- **Depois:** 9 grants centralizados nas 3 roles + 22 usuários com acesso via roles

**Impacto:**
- Zero incidentes de "acesso não funciona" pós-deployment
- Integração contínua, estável e segura entre schemas de dados e aplicação
- Compliance: auditoria facilitada com padrões documentados e rastreáveis
- Modelo replicável para qualquer novo schema Oracle

---

## 📊 Resumo de Impacto

**Economia de tempo operacional mensal:** ~**40+ horas** em automações  
**Redução de erros:** **~99%** em processos automatizados  
**Escalabilidade:** Soluções suportam crescimento sem refatoração  
**Governança:** Processos auditáveis e reproduzíveis

---

## 📫 Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fellipe-oliveira-morsolin-69497a2a/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:fellipemorsolin@gmail.com)

---

*"Medir antes de otimizar. Entender antes de mudar. Testar antes de aprovar."*
