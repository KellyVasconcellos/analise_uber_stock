# 📈 Análise Exploratória e Predição de Tendências: Ações Uber

Este repositório contém um pipeline completo de Análise Exploratória de Dados (EDA) e processamento estatístico aplicado ao histórico de preços das ações da **Uber (UBER)**. O objetivo é transformar dados brutos em insights acionáveis, tratando outliers, normalizando variáveis e analisando a estacionariedade da série temporal.

## 📝 Descrição do Projeto
O projeto aborda o ciclo de vida de um projeto de dados, desde o carregamento e limpeza até a análise de tendências avançada. Através de métodos estatísticos e modelos de regressão, foram identificados padrões de comportamento nos preços de fechamento, permitindo uma visão clara da volatilidade e das tendências de longo prazo do ativo.

## 🛠️ Tecnologias Utilizadas
* **Python 3.x**
* **Pandas & Numpy:** Manipulação e tratamento de dados.
* **Matplotlib & Seaborn:** Visualização de dados e matrizes de correlação.
* **Scikit-learn:** Normalização (StandardScaler) e Regressão Polinomial.
* **Statsmodels:** Suavização LOESS e Teste de Estacionariedade (KPSS).

## 🚀 Etapas do Pipeline
1.  **Limpeza de Dados:** Tratamento de valores ausentes e remoção de duplicatas.
2.  **Engenharia de Atributos:** Criação de variáveis de data (Ano, Mês, Dia) e indicadores financeiros (Retorno Diário e Variação de Preço).
3.  **Tratamento de Outliers:** Aplicação da técnica de **Z-Score** para garantir a integridade estatística.
4.  **Normalização:** Padronização das escalas para permitir comparações justas entre variáveis de volume e preço.
5.  **Análise de Tendência:** Implementação de **Regressão Polinomial (Grau 3)** e **LOESS** para capturar movimentos não-lineares.
6.  **Teste Estatístico (KPSS):** Verificação de estacionariedade para validar a viabilidade de modelos preditivos futuros.

## 📊 Principais Insights
* **Estacionariedade:** O teste KPSS revelou que a série original não é estacionária, exigindo diferenciação (Close_Diff) para análises estatísticas rigorosas.
* **Correlação:** Identificação de variáveis redundantes (como `Adj Close`), otimizando a performance do dataset.
* **Tendências:** O modelo LOESS proporcionou uma suavização mais adaptativa aos ruídos do mercado em comparação à regressão polinomial.

## 📋 Como Executar
1. Clone o repositório:
   ```bash
   git clone [https://github.com/KellyVasconcellos/analise_uber_stock.git]
