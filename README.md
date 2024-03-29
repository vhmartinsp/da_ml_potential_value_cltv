# Avaliação do potencial do cliente da FLO

O projeto visa definir sugestões e recomendação com base em uma análise exploratória de dados (EDA) e um modelo estatístico chamado  BG-NBD, para as atividades de vendas e marketing da FLO, avaliando o valor potencial que os clientes existentes proporcionarão à empresa no futuro. 

## Contexto:

A FLO deseja planejar suas atividades de vendas e marketing a médio e longo prazo e, para isso, deve estimar o valor futuro que os clientes existentes trarão para a empresa

Sobre os dados:

O conjunto de dados consiste em informações obtidas do comportamento de compras anteriores de clientes que fizeram suas últimas compras no OmniChannel (on-line e off-line) entre 2020 e 2021.

Colunas

master_id: Número único do cliente
order_channel: qual canal da plataforma de compras é usado (Android, iOS, Desktop, Mobile, Offline)
last_order_channel: o canal em que a última compra foi feita
first_order_date : A data da primeira compra feita pelo cliente
last_order_date : A data da última compra feita pelo cliente
last_order_date_online : A data da última compra feita pelo cliente na plataforma on-line
last_order_date_offline : A data da última compra feita pelo cliente na plataforma off-line
order_num_total_ever_online : O número total de compras feitas pelo cliente na plataforma on-line
order_num_total_ever_offline: Número total de compras feitas pelo cliente off-line
customer_value_total_ever_offline: O preço total pago pelo cliente em compras off-line
customer_value_total_ever_online: O preço total pago pelo cliente em suas compras on-line
interested_in_categories_12 : Lista de categorias em que o cliente fez compras nos últimos 12 meses

## Funcionalidades: 

O projeto de avaliação do potencial do cliente da FLO envolve carregar e explorar dados de compras anteriores do cliente. Após preparar os dados, aplique modelos estatísticos como BG-NBD e Gamma-Gamma para prever o comportamento futuro do cliente e estimar o valor médio de compra. Essas previsões são usadas para calcular o valor da vida útil do cliente (CLTV) de cada cliente, estimando assim a receita potencial que cada cliente pode gerar para a empresa.

## Como usar: 

Para usar este projeto, siga estas etapas:

- Baixe o arquivo .ipynb: Primeiro, baixe o arquivo do projeto (geralmente com extensão .ipynb) para o seu computador.
- Abra o Google Colab: acesse o Google Colab em seu navegador.
- Carregar um arquivo .ipynb: No menu Arquivo Google Colab, selecione a opção Carregar Notebook. Em seguida, selecione o arquivo .ipynb que você baixou anteriormente.
- Adicione o arquivo flo_data_20k no Notebook do Google Colab
- Importe bibliotecas necessárias: quando o notebook for iniciado, verifique se todas as bibliotecas necessárias foram importadas corretamente. Se necessário, faça as importações apropriadas.
- Execute o notebook: clique em Runtime no menu superior e selecione Executar tudo. Isso executará todas as células do notebook, incluindo download de dados, preparação de dados, aplicação de modelos estatísticos e análise de resultados.


# Evaluation of FLO's customer potential

The project aims to define suggestions and recommendation based on an exploratory data analysis (EDA) and a statistical model called BG-NBD, for FLO's sales and marketing activities by assessing the potential value that existing customers will provide to the company in the future. 

## Context:

FLO wants to plan its sales and marketing activities over the medium to long term and, in order to do so, it must estimate the future value that existing customers will bring to the company

About the data:

The data set consists of information obtained from the past purchasing behavior of customers who made their last OmniChannel purchases (online and offline) between 2020 and 2021.

Columns

master_id: Unique customer number
order_channel: which shopping platform channel is used (Android, iOS, Desktop, Mobile, Offline)
last_order_channel: the channel on which the last purchase was made
first_order_date : The date of the customer's first purchase
last_order_date : The date of the last purchase made by the customer
last_order_date_online : The date of the last purchase made by the customer on the online platform
last_order_date_offline : The date of the last purchase made by the customer on the offline platform
order_num_total_ever_online : The total number of purchases made by the customer on the online platform
order_num_total_ever_offline: Total number of purchases made by the customer offline
customer_value_total_ever_offline: The total price paid by the customer for offline purchases
customer_value_total_ever_online: The total price paid by the customer for their online purchases
interested_in_categories_12 : List of categories in which the customer has shopped in the last 12 months

## Features: 

FLO's customer potential assessment project involves uploading and exploring data from the customer's previous purchases. After preparing the data, apply statistical models such as BG-NBD and Gamma-Gamma to predict future customer behavior and estimate the average purchase value. These predictions are used to calculate the customer lifetime value (CLTV) of each customer, thus estimating the potential revenue each customer can generate for the company.

## How to use: 

- Download the.ipynb file: if you haven't already done so, download the project file, usually with the extension.ipynb, to your computer.
- Open Google Colab.
- Upload the.ipynb file: in Google Colab's "File" menu, select the "Upload from notebook" option. Then choose the.ipynb file you downloaded in the previous step.

- Import the necessary libraries: At the start of the notebook, the necessary libraries should already be imported. Check that the imports are as follows:

import numpy as np;
import pandas as pd;
from sklearn.tree import DecisionTreeClassifier;
from sklearn.model_selection import train_test_split;
from sklearn.metrics import mean_squared_error, accuracy_score;
from sklearn import tree;
import graphviz

- Run the notebook: Click on "Runtime" in the top menu and select "Run All". This will run all the cells in the notebook, including downloading the data, splitting the data, training the model and evaluating the model.
