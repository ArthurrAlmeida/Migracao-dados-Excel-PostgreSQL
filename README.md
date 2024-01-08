# Processo seletivo Rox
Repositorio criado com o intuito de realizar o teste de Eng de Dados Jr na empresa Rox.

<h3> Ferramentas e versôes utilizadas </h3>

  <p>-Ubutu 22</p>
  <p>-Python 3.10.12</p>
  <p>-Spark 3.5</p>
  <p>-PostgreSQL 16.1</p>
  <p>-pgAdmin 4</p>
  <p>-postgresql-42.7.1.jar</p>
  <p>-AWS</p>

<h3> Explicação </h3>

  <p> Tudo foi pensado para ter a melhor performance e mínimo consumo de memória. O Spark é uma ferramenta de ETL poderosa, e se encaixa perfeitamente com o Postgre e com o AWS, assim deixando tudo mais leve e com melhor performance. Durante o processo estive viajando por problemas pessoais e tive que usar um notebook emprestado, com isso criei uma máquina virtual usando VMWare, sistema operacional Ubuntu 22, Spark e Postgre para o ETL e enfim, com os dados prontos, foram inseridos no AWS. </p>

  # Solução

  <h3> Modelagem Conceitual </h3>

![MODELAGEM CONCEITUAL](https://github.com/KnightAlmeida/Teste-Rox/assets/94095714/7b7c0cef-d694-4d76-833e-786b6f8c6437)

<p> A modelagem conceitual tem como objetivo explicar o processo de ETL e tranformação dos dados de CSV para Banco de dados Postgre, ela começa com o arquivo CSV sendo direcionado para o Spark, ferramenta de transformação, depois da transformação ocorre a migração para o Postgre, nele podemos fazer as consultas e modificar os dados, logo após temos duas opções finais, subir para AWS ou implantar na ferramenta de visualização gráfica, que no exemplo foi mostrado o Power BI, mas no teste não foi utilizado</p>

  <h3> O ETL </h3>

  <p> O ETL foi realizado inteiro no Spark, usando PySpark e Postgres, o código usado durante o pescurso está no arquivo chamado 'CÓDIGO FONTE', onde mostra como foi feita a extração e implantação no Postgre.</p>

  <h3> Consultas </h3>

  <p> Logo após ser implantado no Postgre foram feitas as consultas de acordo com o pedido do 'cliente', o código dessas consultas está salvo no arquivo 'QUERYS' onde mostra a solução utilizada para cada consulta de dados pedida. </p>

  <h3> Dados </h3>

  <p> Realizado todo o processo, os dados transformados podem ser encontrados no seguinte link https://s3.console.aws.amazon.com/s3/buckets/rox-dados-arthur?region=sa-east-1&bucketType=general&tab=properties nele tem o backup de todas as tabelas transformadas e prontas para uso. Para visualizar só precisa do PgAdmin, onde abre o arquivo e ele mostra o resultado das tabelas. </p> 

  <h3> Considerações Finais </h3>

  <p> Gostaria de agradecer a equipe Rox por todo apoio e empatia, aprendi muito com o processo seletivo, realizei da forma que sei fazer e que domino, tenho muito a aprender e estou nesse processo para melhorar cada dia mais e o processo seletivo me fez crescer bastante nesse quesito. </p>
  
