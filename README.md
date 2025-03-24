# Detecção de Anomalias com Autoencoder e Isolation Forest

Este projeto implementa um modelo de detecção de anomalias utilizando **Autoencoders** e **Isolation Forest**. O objetivo é identificar padrões anormais em conjuntos de dados, treinando um autoencoder para aprender a representação comprimida dos dados normais e detectando anomalias com base no erro de reconstrução.

## Objetivo

A detecção de anomalias é utilizada em diversas áreas, como segurança da informação, detecção de fraudes e monitoramento de sistemas. Neste projeto, utilizamos:

- **Autoencoder** para modelar padrões normais dos dados.
- **Isolation Forest** para detectar outliers baseando-se na distribuição dos dados.

## Tecnologias Utilizadas

- Python
- Keras (para construção do Autoencoder)
- Scikit-learn (para Isolation Forest)
- NumPy e Matplotlib (para manipulação e visualização dos dados)

## Estrutura do Projeto

1. **Pré-processamento dos Dados**
   - Utiliza-se o dataset MNIST para treinar o autoencoder.
   - Adiciona-se ruído aos dados para simular anomalias.
2. **Treinamento do Autoencoder**
   - O modelo é treinado para reconstruir imagens normais.
   - A diferença entre as imagens originais e reconstruídas é usada para identificar anomalias.
3. **Detecção de Anomalias**
   - Mede-se o erro de reconstrução (MSE) para detectar outliers.
   - O Isolation Forest é usado para reforçar a detecção de anomalias nos dados.
