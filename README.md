# Análise de Dados de Ecommerce com Regressão Linear

## Contexto

A análise foi realizada para um ecommerce com sede em Nova York que oferece roupas e sessões de consultoria de estilo. O objetivo é determinar se a empresa deve focar mais no desenvolvimento de seu aplicativo móvel ou no site, considerando o impacto das duas plataformas nas despesas dos clientes.

## Importação de Dados

O conjunto de dados utilizado inclui informações sobre:

- **Avg. Session Length**: Tempo médio das sessões de consultoria na loja.
- **Time on App**: Tempo médio gasto no aplicativo móvel.
- **Time on Website**: Tempo médio gasto no site.
- **Length of Membership**: Duração da associação do cliente.

Os dados foram carregados a partir de um arquivo CSV e explorados para análise inicial.

## Análise Exploratória

A análise exploratória revelou que o "Tempo de Associação" é a variável mais correlacionada com o valor anual gasto pelos clientes. Visualizações dos dados confirmaram que clientes com maior tempo de associação tendem a gastar mais.

## Preparação dos Dados

Os dados foram divididos em conjuntos de treinamento e teste, e um modelo de regressão linear foi treinado para prever o valor anual gasto com base nas características numéricas dos clientes.

## Resultados do Modelo

Os coeficientes do modelo mostraram que:

- **Tempo no App**: Um aumento de 1 unidade está associado a um aumento de $38,59 no gasto anual.
- **Tempo no Site**: Um aumento de 1 unidade está associado a um aumento de $0,19 no gasto anual.
- **Tempo de Associação**: Um aumento de 1 unidade está associado a um aumento de $61,27 no gasto anual.

O "Tempo de Associação" mostrou ter o maior impacto no gasto anual, seguido pelo "Tempo no App".

## Avaliação do Modelo

O modelo foi avaliado usando três métricas de regressão:

- **Erro Absoluto Médio (MAE)**: Forneceu uma média dos erros absolutos.
- **Erro Médio Quadrático (MSE)**: Avaliou o erro quadrático médio.
- **Raiz do Erro Quadrático Médio (RMSE)**: Ofereceu uma interpretação das unidades de gasto.

As métricas confirmaram a eficácia do modelo na previsão dos gastos anuais.

## Conclusão

A análise sugere que a empresa deve focar em estratégias para aumentar o tempo de associação dos clientes, pois esta variável tem o maior impacto no gasto anual. Entre o site e o aplicativo, o investimento no aplicativo móvel é mais vantajoso devido ao seu maior coeficiente. Portanto, recomenda-se priorizar o desenvolvimento e aprimoramento do aplicativo para maximizar os gastos dos clientes.
