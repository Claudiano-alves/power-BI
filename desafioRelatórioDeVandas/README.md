# Relatório de Vendas no Power BI

Este projeto faz parte de um **desafio de projeto** realizado na **(DIO)**, com o objetivo de criar um **Relatório de Vendas** utilizando o Power BI. 

## Objetivo
O objetivo deste trabalho foi desenvolver um relatório interativo e dinâmico que permita a análise das vendas de uma empresa, fornecendo insights sobre o desempenho de vendas, produtos, e descontos, além de facilitar a visualização de tendências ao longo do tempo.

## Tabelas Utilizadas
O modelo de dados foi criado com base em um **Star Schema** composto pelas seguintes tabelas:
- **f_vendas**: Tabela fato contendo os registros de vendas realizadas.
- **d_produtos**: Tabela dimensão com informações sobre os produtos.
- **d_produtosDetalhes**: Detalhes adicionais dos produtos.
- **d_calendario**: Tabela de calendário para análise temporal das vendas.
- **d_descontos**: Informações sobre os descontos aplicados nas vendas.

## Funcionalidades
- Visualizações interativas com gráficos de barras, linhas e mapas.
- Filtros dinâmicos para permitir a análise por período, produto e descontos.
- Medidas em DAX para cálculos de total de vendas, ticket médio e variações de desempenho.

Este relatório foi desenvolvido para atender às necessidades de visualização e tomada de decisão com base em dados reais de vendas.
