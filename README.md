Projeto de Machine Learning — Energy Efficiency Dataset

Este projeto tem como objetivo analisar, modelar e prever variáveis relacionadas à eficiência energética de edificações utilizando técnicas de Análise Exploratória de Dados (EDA), regressão, classificação, avaliação de modelos e otimização.

O trabalho segue a estrutura recomendada para projetos completos de Data Science, incluindo preparação dos dados, visualizações, modelagem e validação rigorosa.

🗂️ Sumário

Descrição do Projeto

Tecnologias Utilizadas

Estrutura do Projeto

Base de Dados

Análise Exploratória (EDA)

Modelos de Regressão

Modelos de Classificação

Métricas Utilizadas

Como Executar

Resultados

Próximos Passos

📌 Descrição do Projeto

O objetivo do projeto é revisar os fatores que influenciam a eficiência energética a partir de características físicas das edificações, e construir modelos capazes de:

🔹 Regressão

Prever valores numéricos como:

Heating Load

Cooling Load

🔹 Classificação

Classificar as edificações em faixas de eficiência energética, como:

Baixa eficiência

Média eficiência

Alta eficiência

Para isso, utilizamos técnicas modernas de machine learning e validação estatística.

🛠️ Tecnologias Utilizadas

Python 3.10+

Pandas

NumPy

Matplotlib / Seaborn

Scikit-learn

Jupyter Notebook

PyCaret (opcional)

📁 Estrutura do Projeto
📦 energy-efficiency-ml
├── data/
│   └── energy_efficiency.csv
├── notebooks/
│   └── análise_e_modelagem.ipynb
├── src/
│   └── preprocessing.py
│   └── models.py
│   └── evaluation.py
├── README.md
└── requirements.txt

📊 Base de Dados

O conjunto de dados contém características construtivas das edificações e suas respectivas cargas térmicas.
Exemplos de variáveis:

Wall Area

Roof Area

Overall Height

Glazing Area

Orientation

Heating Load (alvo regressão)

Cooling Load (alvo regressão)

🔍 Análise Exploratória (EDA)

A EDA incluiu:

Verificação de valores ausentes

Estatísticas descritivas

Correlações (Heatmap)

Pairplots

Boxplots para detectar outliers

Gráficos de dispersão entre variáveis e cargas térmicas

Principais conclusões:

Algumas variáveis possuem forte correlação com cargas térmicas.

Não há dados faltantes no dataset original.

Outliers são reduzidos e não comprometem o modelo.

🤖 Modelos de Regressão

Os seguintes modelos foram treinados:

1. Regressão Linear

Modelo base

Fácil interpretação

2. Regressão Polinomial

Expansão via PolynomialFeatures

Grau utilizado: 2 (melhor custo-benefício)

3. Random Forest Regressor

Modelo não linear forte

Captura interações complexas

4. Gradient Boosting Regressor

Melhor performance geral

🧮 Modelos de Classificação

Criamos classes baseadas nos tercis do Heating Load e aplicamos:

Logistic Regression

KNN

Random Forest Classifier

Gradient Boosting Classifier

SVM

Resultados mostraram que Random Forest e Gradient Boosting têm a melhor acurácia.

📏 Métricas Utilizadas
Para Regressão:

RMSE

MAE

R²

MSE

Para Classificação:

Acurácia

F1-score

Matriz de confusão

Relatório de classificação

▶️ Como Executar

1. Executar notebook
jupyter notebook

🏁 Resultados

Modelos polinomiais melhoram a regressão, mas Random Forest e Gradient Boosting apresentam menor erro.

Modelos baseados em árvores são superiores para prever cargas térmicas.

A classificação atinge bons resultados com Random Forest e SVM.

🚀 Próximos Passos

Implementar tuning avançado com Optuna.

Criar API com FastAPI para predição online.

Implementar dashboard com Streamlit.

Expandir dataset com features novas.
