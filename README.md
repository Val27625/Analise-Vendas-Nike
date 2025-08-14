# Analise-Vendas-Nike

Markdown

# Projeto de Análise de Dados de Vendas da Nike

## 1. Coleta de Dados

O conjunto de dados principal para esta análise foi o `Nike_Sales_Uncleaned.csv`, que contém informações de vendas de uma empresa de varejo. Para complementar a análise e obter uma visão mais ampla, foram levantadas as seguintes fontes de dados públicas e não confidenciais:

-   **Dados Climáticos (INMET):** Para correlacionar a demanda por produtos com as condições climáticas.
-   **Dados de Eventos Esportivos (Sites de Ligas):** Para identificar picos de vendas relacionados a grandes eventos.
-   **Dados Demográficos (IBGE):** Para entender o contexto populacional e econômico de cada região.

O método de coleta foi o download direto do arquivo CSV e o levantamento de outras fontes públicas para futuras análises.

## 2. Modelagem (Análise Exploratória de Dados)

A fase de modelagem consistiu na Análise Exploratória de Dados (EDA) usando Python e a biblioteca Pandas. As principais etapas foram:

1.  **Limpeza e Pré-processamento:**
    -   Padronização dos nomes de regiões (ex.: 'bengaluru' para 'Bangalore').
    -   Conversão do campo `Order_Date` para o tipo de dado de data.
    -   Tratamento de valores ausentes, preenchendo as colunas `Units_Sold` e `MRP` com a mediana.
    -   Criação do arquivo `Nike_Sales_Cleaned.csv` para a análise final.

2.  **Análise Descritiva e Visualizações:**
    -   Geramos estatísticas descritivas para as colunas numéricas (`Profit`, `Revenue`).
    -   Criamos diversos gráficos para visualizar a distribuição e as tendências dos dados, incluindo lucro por linha de produto, sazonalidade mensal, e distribuição de vendas por canal e região.

## 3. Conclusões

A análise exploratória de dados revelou insights valiosos que podem ser usados para otimizar as operações da empresa:

* **Estratégia de Produto:** A linha de **Training** é a mais lucrativa, justificando um foco maior em marketing e desenvolvimento. A linha de **Running**, com menor lucro, precisa de uma investigação mais profunda.
* **Otimização de Estoque:** A sazonalidade identificada no lucro mensal é um fator crítico. A empresa pode usar essa informação para planejar o estoque, garantindo que haja produtos suficientes em períodos de pico e evitando excesso em períodos de baixa.
* **Performance dos Canais e Regiões:** A distribuição de vendas equilibrada entre **Online** e **Retail** valida a estratégia omnicanal da empresa. A análise regional destaca a importância de focar em mercados mais lucrativos como **Delhi** e **Bangalore**, ao mesmo tempo em que se busca melhorar o desempenho em outras áreas.

Essas conclusões servem como base para a tomada de decisões e podem ser aprofundadas com modelos preditivos para previsão de demanda e alocação de recursos.

---
