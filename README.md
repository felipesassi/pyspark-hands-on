# PySpark - Fundamentos e aplicações

A ideia do *notebook* desse repositório é apresentar os fundamentos de uso da API *Python* para *Spark*. Vamos verificar os principais comandos, e entender o que são ações, transformações, execução *lazy* e as famosas DAG's geradas pelo *Spark* (essa última parte de uma forma mais superficial).

Após essa breve introdução e explanação dos conceitos, nós iremos simular uma utilização em um problema de negócio, para facilitar a assimilação de tudo que foi visto.

Esse *notebook* pode ser usado em um ambiente *Databricks*, o qual conta com algumas funcionalidades que facilitam nosso trabalho diário.

O *notebook* também pode ser acessado pelo seguinte *link*: [PySpark Hands-on](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1947510454734791/317198982518282/8080406957112694/latest.html).

## Pontos importantes sobre a interface do *Databricks*

A aba na lateral direita nos permite:

- criar *notebooks*, a partir da opção *create*;
- importar dados, também na opção *create*. Essa importação é feita a partir de uma interface gráfica, muito simples de ser utilizada (vale a pena o teste);
- criação de um *cluster* na opção *compute*. Todo *notebook* deve ser associado a um *cluster* para execução.

## Dados utilizados

Os dados utilizados estão dispobilizados no *Kaggle*:

- Link para *download*: [Conjunto de dados](https://www.kaggle.com/olistbr/brazilian-ecommerce?select=olist_order_payments_dataset.csv)

Nesse projeto vamos utilizar as tabelas:

- *olist_customers_dataset.csv*;
- *olist_order_payments_dataset.csv*;
- *olist_orders_dataset.csv*.

### Contexto dos dados

"*This dataset was generously provided by Olist, the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners. After a customer purchases the product from Olist Store a seller gets notified to fulfill that order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where he can give a note for the purchase experience and write down some comments.*"

### Link entre os dados

![databases](https://i.imgur.com/HRhd2Y0.png)

## Referências úteis

- Documentação: [Documentação PySpark](https://spark.apache.org/docs/latest/api/python/index.html);
- Criando tabelas: [Criação de tabelas no databricks](https://docs.databricks.com/data/tables.html).
