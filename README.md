# Databricks_Overview
Repositório do curso da plataforma DIO - Microsoft AI for Tech - Azure Databricks

Azure Databricks: Usando um Notebook para Analisar Dados
Notebooks são ambientes interativos onde você pode escrever e executar código para análise de dados, visualização e machine learning.

Criando um Notebook:
No Databricks, vá para Workspace > Users > [Seu usuário].

Clique com o botão direito e selecione "Create > Notebook".

Dê um nome, escolha a linguagem (Python, SQL, Scala ou R) e selecione o cluster.

Exemplo de análise com Python e Spark:
python
Copiar
Editar
# Carregando dados CSV do Data Lake (ou de uma URL pública)
df = spark.read.csv("dbfs:/mnt/datalake/exemplo.csv", header=True, inferSchema=True)

# Visualizando as primeiras linhas
display(df)

# Estatísticas básicas
df.describe().show()

# Agrupamento por uma coluna
df.groupBy("categoria").count().show()
Você também pode criar visualizações gráficas diretamente no notebook usando a função display(), ideal para análise exploratória.

C
