# Pipeline de Engenharia de Dados

## Projeto integrador desenvolvido como estudo prático de **Engenharia de Dados**, simulando a construção de uma arquitetura moderna de dados para uma empresa do setor automotivo.

## 🎯 Contexto do Projeto

Este projeto simula um cenário real de negócio em que a empresa fictícia **NovaDrive** dependia de planilhas **Excel** para controle operacional e acompanhamento de vendas.

É solicitado uma solução que permita:

- centralizar os dados operacionais
- automatizar o processamento de dados
- disponibilizar informações estruturadas para análise
- apoiar a tomada de decisão estratégica

A proposta deste projeto foi **projetar e implementar um pipeline de dados completo**, desde a ingestão até a visualização analítica.

---

## 🚀 Objetivos

O projeto tem como objetivo desenvolver uma **arquitetura de dados moderna** capaz de:

- realizar ingestão automatizada de dados operacionais
- orquestrar pipelines de dados
- transformar e modelar dados para análise
- garantir organização e qualidade dos dados
- disponibilizar informações em dashboards analíticos

---

## 🔌 Conexão e Exploração de Dados

O pipeline inicia com a conexão ao banco de dados **PostgreSQL**, responsável por armazenar os dados operacionais da empresa.

Nessa etapa foram realizadas:

- conexão com banco de dados
- execução de consultas SQL
- exploração da estrutura dos dados
- entendimento do modelo operacional

Essa fase permite compreender a estrutura da base antes da construção do pipeline.

---

## 🔄 Pipeline de Dados

O pipeline foi construído utilizando uma abordagem **ELT (Extract, Load, Transform)**.

Inicialmente os dados são carregados para o **Data Warehouse** e posteriormente transformados na camada analítica.

Durante essa etapa foram implementados:

- criação de **DAGs no Apache Airflow**
- definição de dependências entre tarefas
- criação de conexões com fontes de dados
- execução automatizada do pipeline
- testes de carga incremental
- diagnóstico e resolução de erros de execução

O **Airflow** é responsável por orquestrar todo o fluxo de dados.

---

## ⚙️ Orquestração com Apache Airflow

O ambiente de orquestração foi configurado utilizando **Docker containers** executados em uma instância **AWS EC2**.

Durante o desenvolvimento foram realizados ajustes técnicos importantes, incluindo:

- correção de incompatibilidade com **Airflow 3**
- ajuste de **Dynamic Task Mapping**
- diagnóstico de erro relacionado ao **Serialized Timetable**
- limpeza e reinicialização do banco de metadados do Airflow
- organização do ambiente containerizado

Também foi explorada a arquitetura interna do Airflow, incluindo componentes como:

- Scheduler
- DAG Processor
- API Server

---

## 📈 Dashboard Analítico

Para consumo dos dados foi desenvolvido um dashboard utilizando **Looker Studio**, com o objetivo de fornecer indicadores estratégicos para a área de vendas da empresa.

O dashboard apresenta métricas como:

- receita total de vendas
- quantidade total de vendas
- distribuição de vendas por estado
- desempenho das concessionárias

A imagem do dashboard criado neste
projeto encontra-se em:

`assets/dashboard_vendas.png`

---

## 🛠 Tecnologias Utilizadas

- Python
- PostgreSQL
- Apache Airflow
- Snowflake
- dbt
- Docker
- AWS EC2
- Looker Studio

---

## 💡 Principais Aprendizados

Durante o desenvolvimento do projeto foram explorados diversos conceitos fundamentais de engenharia de dados, incluindo:

- construção de pipelines de dados
- orquestração de workflows
- modelagem dimensional
- integração entre banco operacional e data warehouse
- uso de ferramentas modernas de transformação de dados
- containerização de ambientes
- execução de pipelines em infraestrutura cloud

---

## 👩‍💻 Autora

Janyne Soares

Projeto desenvolvido como estudo prático de Engenharia de Dados, também apresentado como **Projeto Integrador da Pós-Graduação em Ciência de Dados pela Universidade Tecnológica Federal do Paraná (UTFPR)**.

-Baseado em estudos e práticas de cursos na área de Engenharia de Dados.
