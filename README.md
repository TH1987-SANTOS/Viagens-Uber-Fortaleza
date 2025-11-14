### 🧠 Predição de Preços de Corridas Uber — Regressão com ML
Machine Learning • Data Cleaning • Feature Engineering • Modelos Preditivos

Este projeto realiza uma análise completa e profissional para prever o valor das corridas da Uber utilizando modelos de Regressão Linear e Random Forest.
Inclui limpeza de dados, pré-processamento com pipelines, avaliação avançada de modelos e exportação dos modelos treinados para uso posterior.

### 📌 Objetivos do Projeto

Construir um pipeline de Machine Learning totalmente replicável.

Tratar dados sujos, incluindo remoção da coluna técnica Unnamed: 0.

Criar um fluxo robusto de pré-processamento para variáveis numéricas e categóricas.

Treinar e comparar dois modelos:

Linear Regression

Random Forest Regressor

Avaliar as métricas de regressão:

MAE

RMSE

R²

Salvar os modelos treinados usando joblib.

### 📂 Estrutura do Notebook

O notebook segue um formato profissional dividido em seções:

1. Carregamento e Limpeza dos Dados

Remoção da coluna Unnamed: 0

Conversão de valores faltantes

2. Análise Exploratória Inicial

Identificação dos tipos de variáveis

Visualização e descrição básica

3. Preparação das Variáveis

Separação em X e y

Seleção automática das features numéricas e categóricas

4. Pré-Processamento com ColumnTransformer

Imputação

One-Hot Encoding

Padronização das variáveis numéricas

5. Treinamento dos Modelos

Pipeline Linear Regression

Pipeline Random Forest

train_test_split com 20% para teste

6. Avaliação dos Modelos

Para cada modelo, são calculadas:

Métrica	Descrição
MAE	Erro médio absoluto – facilidade de interpretação
RMSE	Erro quadrático médio – penaliza grandes erros
R²	Quanto o modelo explica da variação dos dados

Um DataFrame final apresenta os resultados lado a lado.

7. Exportação dos Modelos

Os modelos são salvos em:

models/model_linear_regression_safe.joblib
models/model_random_forest_safe.joblib

### 📊 Comparação dos Modelos (Resumo Conceitual)

Linear Regression

Simples, rápida e interpretável.

Ideal quando relações lineares predominam.

Random Forest Regressor

Modelo robusto baseado em árvores.

Captura relações não lineares e interações entre variáveis.

Normalmente fornece melhor desempenho geral.

➤ A interpretação completa dos resultados fica no notebook na seção "Avaliação dos Modelos".

### 📈 Importância das Variáveis (Opcional)

Caso seja incluído:

Gráfico mostrando quais features influenciam mais o preço.

Útil em análises de negócio e insights.

### 🏁 Conclusão (Resumo)

O projeto implementou um fluxo completo de Machine Learning, desde a limpeza dos dados até a comparação entre dois modelos preditivos. A abordagem com pipelines garante reprodutibilidade e segurança no treinamento, evitando erros comuns como desalinhamento de colunas.

O Random Forest tende a oferecer desempenho superior em cenários reais, mas a escolha final depende das métricas observadas no dataset.