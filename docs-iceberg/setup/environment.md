---
title: Configuração do Ambiente
---

## Java e JAVA_HOME

O PySpark requer Java (JDK). Em distribuições baseadas em Debian/Ubuntu:

```bash
sudo apt-get update
sudo apt-get install -y openjdk-17-jdk
```

Defina `JAVA_HOME` (exemplo para OpenJDK 17):

```bash
echo "export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64" >> ~/.bashrc
echo "export PATH=\$JAVA_HOME/bin:\$PATH" >> ~/.bashrc
source ~/.bashrc
java -version
```

Se estiver em WSL, execute os comandos dentro do Ubuntu/WSL.

## Jupyter Lab

Inicie o Jupyter Lab com o ambiente virtual:

```bash
uv run jupyter lab
```

Selecione o kernel `.venv` ao abrir o notebook `notebooks/spark-iceberg.ipynb`.

## Executar Spark + Iceberg

Com Java configurado e kernel correto, os exemplos do notebook devem executar normalmente.


