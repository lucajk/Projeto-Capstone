# Projeto-Capstone
## Relatório 

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
 No dataset possuí as seguintes colunas:
 * ride_id:
   Uma coluna do tipo varchar e única, onde se encontra os ids dos usuários.
 * started_at:
   Coluna do tipo date, indica o horário de início das viagens
 * ended_at:
   Coluna do tipo date, indica o horário do fim das viagens
 * start_station_name: Indica o nome da estação inicial
 * ended_station_name: Indica o nome da estação final
 * end_station_id: Indica o Id da estação final
 * start_lat e lng: Indica a latitude e longitude das estações iniciais
 * end_lat e lng: Indica a latitude e longitude das estações finais
 * member_casual: Indica se o usuário é member ou casual 
 
## 3. Preparação dos Dados
## Limpeza dos dados
  Antes de qualquer limpeza, retirei a coluna "ride_id" e "rideable_type" por não ser tão útil para nossas análises.
  Foi removido qualquer linha que houvesse valores em branco que seriam essenciais para a análise, como data e hora de partidade e chegada,
  como também localização dos pontos de compartilhamento.
## Formatação
   Cada coluna foi formatada a partir de seu real valor, como data, numerico, etc.
     
## Recursos categóricos de codificação label encoding
   A coluna "member_casual" passou pelo processo de label-encoding a fim de otimizar e facilitar a análise categoricamente.
     
## 4.Modelagem
    Durante a aquisição de parâmetros utilizei do método de regressão linear, onde tracei uma reta afim de projetar novos valores de acordo com o tempo de duração das viagens e quantidade de viagens realizadas.

## 5 Avaliação
    Nesta etapa, calculei o erro absoluto na previsão linear, onde obtive uma média de erro absoluto de 23 unidades, isso indica um bom modelo de previsão, já que essa quantidade não impacta sgnificavelmente nossa análise.
