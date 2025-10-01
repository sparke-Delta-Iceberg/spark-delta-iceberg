---
title: Operações CRUD com Apache Iceberg e DeltaLake + Spark(Airbnb)
---

## Operações CRUD

As demonstrações de CRUD usando Apache Iceberg com PySpark estão no notebook `notebooks/spark-iceberg/spark-iceberg.ipynb`.

No MkDocs: [Notebooks → Spark + Iceberg](../notebooks/spark-iceberg/spark-iceberg.ipynb).
No MkDocs: [Notebooks → Spark + Delta Lake](../notebooks/spark-delta-lake/spark-delta-lake.ipynb).

Passos gerais:

1. Iniciar a sessão Spark (ver [Configuração do Ambiente](../setup/environment.md)).
2. Criar/Carregar tabela referente ao dataset Airbnb.
3. Executar inserções/atualizações/remoções conforme exemplos no notebook.

Para executar o notebook:

- Inicie o Jupyter Lab: `uv run jupyter lab`
- Selecione o kernel `.venv`
- Garanta que o Java esteja instalado e `JAVA_HOME` configurado (ver [Configuração do Ambiente](../setup/environment.md)).


