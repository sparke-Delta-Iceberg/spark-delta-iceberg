## Projeto Spark com apache iceberg e delta lake

Projeto desenvolvido para demonstração do Apache Spark Local (pyspark) gravando arquivos no formato Apache Iceberg também de forma local.

Utilize o WSL do Windows 11 ou alguma outra distro Linux. Não utilize ambiente Windows, pois será necessário efetuar várias configurações adicionais para funcionar.

Para este laboratório foi utilizado o Linux Ubuntu 24.04.

**Para utilização dos notebooks, é necessário possuir java 17 instalado e configurado**

![Versao Linux](/assets/linux-version.png)

Projeto python inicializado com o [UV](https://github.com/astral-sh/uv).

Comandos utilizados para setup do ambiente:

```bash copy
uv init
uv venv
source .venv/bin/activate
uv add pyspark==3.5.3 jupyterlab ipykernel delta delta-spark
```

Os exemplos de código pyspark/python para instanciar o Spark, bem como criar e manipular uma tabela Apache Iceberg, está no arquivo `notebooks/spark-iceberg.ipynb`.

**Nota:** Antes de executar o arquivo citado acima, não esqueça de selecionar o seu ambiente virtual (.venv) como Kernel do seu jupyter notebook.

![image](https://github.com/user-attachments/assets/6394e5b6-c51e-4245-bad2-450d864e422a)

Nota 2: O arquivo .ipynb (jupyter notebook) foi executado dentro do VS Code.

## Documentação (MkDocs)

Servir a documentação localmente:

```bash
uv sync
uv run mkdocs serve
```

Depois, acesse o endereço exibido no terminal (geralmente `http://127.0.0.1:8000`).

No site, o notebook aparece no menu: Notebooks → Spark + Iceberg.

Build (opcional):

```bash
uv run mkdocs build
```

Links e referências sobre a compatibilidade da versão do Apache Spark (pyspark) e Apache Iceberg:

[https://iceberg.apache.org/spark-quickstart/](https://iceberg.apache.org/spark-quickstart/) <br>
[https://mvnrepository.com/artifact/org.apache.iceberg/iceberg-spark-runtime-3.5](https://mvnrepository.com/artifact/org.apache.iceberg/iceberg-spark-runtime-3.5) <br>
[https://medium.com/@tglawless/developing-with-apache-iceberg-pyspark-2727957f173f](https://medium.com/@tglawless/developing-with-apache-iceberg-pyspark-2727957f173f)
