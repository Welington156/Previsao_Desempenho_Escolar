# 🎓 TCC – Previsão do Desempenho Escolar do 9º Ano (SAEB 2021)

Este repositório contém o projeto de monografia de Bacharelado em Ciência da Computação, intitulado “Previsão do Desempenho Escolar do 9º Ano em Escolas Públicas com Base em Fatores Socioeconômicos e Culturais”, apresentado ao IFNMG – Campus Montes Claros.

## 📋 Descrição do Projeto

Objetivo: Analisar como fatores socioeconômicos e culturais influenciam as notas de Matemática do 9º ano em escolas públicas, e desenvolver modelos preditivos de proficiência ("Proficiente" vs. "Insuficiente").

Fonte de dados: SAEB 2021 (INEP), base com 1.886.179 registros de alunos.

Categorias de saída: notas contínuas convertidas em binário para facilitar interpretação e modelagem.

## 🔍 Metodologia

Análise Exploratória (AED): limpeza, padronização e visualizações das 31 questões socioeconômico‑culturais.

Seleção de Características: algoritmo CART (Minitab) para escolher as 15 variáveis mais relevantes, reduzindo perda de dados a 19,19%.

Balanceamento: aplicação de SMOTE e RandomUnderSampler para tratar desbalanceamento entre classes.

Modelagem Preditiva: testes com:

Regressão Logística (baseline e otimizada via Grid Search)

Random Forest (baseline e otimizada via Grid Search)

Avaliação: métricas de Acurácia, Precisão, Recall e F1‑Score e análise de matrizes de confusão.

## 📈 Resultados Principais

Fatores Positivos: participação em atividades extracurriculares e estudo fora da escola associados a maior proficiência.

Fatores Negativos: idade elevada, reprovações anteriores e baixa condição socioeconômica correlacionam‑se com insuficiência.

Desempenho dos Modelos (SMOTE):

Regressão Logística: Acurácia ~65%, F1‑Score “Proficiente” 39%, “Insuficiente” 75%.

Random Forest: Acurácia ~67%, com recall de 70% para classe “Insuficiente”.

Insights para Políticas Educacionais: priorizar programas de apoio a alunos mais velhos e de baixa renda; incentivar atividades extracurriculares.
