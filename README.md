# Projeto-Capstone
## Relatótio 

## 1. Entendimento do problema:
O projeto tem como objetivo analisar dados de compartilhamento de bicicletas, a fim de realizar uma ação contra a mudança climática global.

O conjunto de dados provém do Google Data Analytics course on Coursera, os dados tem origem fictícia e contém informações sobre compartilhamento de bicicletas de abril de 2021 até março de 2022. A meta do projeto é estabelecer como atrair clientes casuais para o plano anual, de forma que o cliente use mais um meio de transporte não poluente e que por consequência degrade o meio ambiente.

Mia informações sobre o Dataset podem ser encontradas aqui: [https://www.kaggle.com/datasets/evangower/cyclistic-bike-share?resource=download]

## ESCOPO

* O escopo deste projeto é criar gráficos de maneira que o dono da empresa consiga visualizar de maneira mais íntegra as mudanças necessárias para atrair novos clientes
* Utilizei ferramentas como SQL, Excel e Power BI com o intuito de agilizar e otimizar a análise dos dados.

## Plano

Segui os estágios de análise do método CRISP-DM, documentando detalhadamente cada etapa de análise.

## 2.  Entendimento dos dados
 ### Dados Brutos

 Para obter mais informações dos dados consultar link disponibilizado acima.
 Estes dados foram encontrados no Kaggle e disponibilizados pelo Google Data Analytics course on Coursera.
 Há um total de 284043 linhas antes de qualquer filtragem.
 
## 3. Preparação dos Dados
 ### Limpeza dos dados
     Antes de qualquer limpeza, retirei a coluna "ride_id" e "rideable_type" por não ser tão útil para nossas análises.
     Foi removido qualquer linha que houvesse valores em branco que seriam essenciais para a análise, como data e hora de partidade e chegada,
     como também localização dos pontos de compartilhamento.
 ### Formatação
     Cada coluna foi formatada a partir de seu real valor, como data, numerico, etc.
     
 ### Recursos categóricos de codificação label encoding
     A coluna "member_casual" passou pelo processo de label-encoding a fim de otimizar e facilitar a análise categoricamente.
     
## 4.Modelagem
    Durante a aquisição de parâmetros utilizei do Método dos Mínimos Quadrado Least Squares, onde tracei uma reta afim de projetar novos valores de acordo com os dias da semana e quantidade de viagens realizadas.

     
