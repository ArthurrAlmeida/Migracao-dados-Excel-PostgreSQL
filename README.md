# Migração de dados Excel para PostgreSQL

  <p> Tudo foi pensado para ter a melhor performance e mínimo consumo de memória. O Spark é uma ferramenta de ETL poderosa, e se encaixa perfeitamente com o Postgre e com o AWS, assim deixando tudo mais leve e com melhor performance. Durante o processo estive viajando por problemas pessoais e tive que usar um notebook emprestado, com isso criei uma máquina virtual usando VMWare, sistema operacional Ubuntu 22, Spark e Postgre para o ETL e enfim, com os dados prontos, foram inseridos no AWS. </p>

## Desenho
![1](https://github.com/user-attachments/assets/ec75bfa8-6520-44a6-9178-12ed9226adb5)

## Tecnologias

  <p>-Ubutu 22</p>
  <p>-Python 3.10.12</p>
  <p>-Spark 3.5</p>
  <p>-PostgreSQL 16.1</p>
  <p>-pgAdmin 4</p>
  <p>-postgresql-42.7.1.jar</p>
  <p>-AWS</p>



## Solução

<p> Tem como objetivo a tranformação dos dados de CSV para Banco de dados Postgre, ela começa com o arquivo CSV sendo direcionado para o Spark, ferramenta de transformação, depois da transformação ocorre a migração para o Postgre, nele podemos fazer as consultas e modificar os dados, logo após temos duas opções finais, subir para AWS ou implantar na ferramenta de visualização gráfica, que no exemplo foi mostrado o Power BI, mas no teste não foi utilizado</p>

  <h3> O ETL </h3>

  <p> O ETL foi realizado inteiro no Spark, usando PySpark e Postgres, o código usado durante o pescurso está no arquivo chamado 'CÓDIGO FONTE', onde mostra como foi feita a extração e implantação no Postgre.</p>

  <h3> Consultas </h3>

  <p> Logo após ser implantado no Postgre foram feitas as consultas de acordo com o pedido do 'cliente', o código dessas consultas está salvo no arquivo 'QUERYS' onde mostra a solução utilizada para cada consulta de dados pedida. </p>

  <h3> Dados </h3>

  <p> Os dados transformados podem ser encontrados no seguinte link https://s3.console.aws.amazon.com/s3/buckets/rox-dados-arthur?region=sa-east-1&bucketType=general&tab=properties nele tem o backup de todas as tabelas transformadas e prontas para uso. Para visualizar só precisa do PgAdmin, onde abre o arquivo e ele mostra o resultado das tabelas. </p> 
