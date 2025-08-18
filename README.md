# Desafio Técnico - Engenheiro(a) de Dados Sênior (Winnin)

Este repositório contém a minha solução para o desafio técnico de Engenharia de Dados Sênior proposto pela Winnin. O projeto está dividido em duas partes, conforme solicitado no enunciado.

---

## Estrutura do Repositório

- **/notebooks**: Contém os 4 notebooks PySpark desenvolvidos para a **Parte 1** do desafio (Implementação Prática).
- **/architecture**: Contém a documentação da proposta de arquitetura para a **Parte 2** do desafio, incluindo diagramas e princípios de design.
- **README.md**: Este arquivo, com as instruções gerais do projeto.

---

## Parte 1: Implementação Prática com Databricks

Os notebooks na pasta `/notebooks` foram desenvolvidos para serem executados no Databricks Community Edition e resolvem os exercícios práticos propostos.

### Ordem de Execução

Os notebooks devem ser executados na seguinte ordem:

1.  `1 - create_table_creators_scrape_wiki.py`
2.  `2 - create_table_posts_creator.py`
3.  `3 - create_table_user_yt_from_wikipedia_api.py`
4.  `4 - analyze_creators.py`

### Pré-requisitos para Execução

- Um ambiente Databricks (Community Edition ou superior).
- Os arquivos `wiki_pages.json.gz` e `posts_creator.json.gz` devem ser carregados para um local acessível pelo Databricks (ex: Unity Catalog Volumes ou DBFS).
- Os caminhos dos arquivos de input nos widgets dos notebooks 1 e 2 devem ser atualizados para refletir o local onde os arquivos foram carregados.

---

## Parte 2: Proposta de Arquitetura

A proposta de arquitetura para um pipeline de dados contínuo e escalável está detalhada no seguinte documento:

- **[Clique aqui para ver a Proposta de Arquitetura](./architecture/architecture.md)**

O documento aborda os seguintes tópicos:
- Escolha do Orquestrador
- Modelagem de Dados (Medallion e Star Schema)
- Estratégias de Extração de Dados (Inicial e Incremental)
- Etapas do Pipeline e Runbooks Operacionais
- Monitoramento, Qualidade e Governança (SLAs, SLOs, CLOs)
- Boas Práticas de Engenharia de Software (CI/CD, IaC)

---

Obrigado pela oportunidade!