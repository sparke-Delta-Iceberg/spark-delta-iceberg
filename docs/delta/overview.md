---
title: Visão Geral do Delta Lake
---

## O que é Delta Lake?

Apache Delta Lake é um formato de armazenamento open source otimizado para dados em larga escala.  
Ele roda em cima do Apache Parquet e adiciona recursos como transações ACID, controle de versão de dados (time travel) e gestão confiável de pipelines de dados.  
É amplamente usado junto com o Apache Spark e integra-se bem em arquiteturas de Data Lakehouse.

### Benefícios

- Evolução de schema confiável (adicionar ou modificar colunas sem quebrar o histórico)
- Time travel: consultar dados em versões passadas por meio de snapshots
- Operações ACID: garante consistência em leituras e escritas concorrentes
- Otimizações de leitura e escrita com índices e compactação automática
- Integração com Spark, Presto, Trino e outras ferramentas
