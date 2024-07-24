# 📊 Análise de Sentimentos em Avaliações de Produtos usando Amazon AWS [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Neste Projeto para o Curso de IA do Lab DIO, usei o SageMaker Canvas para criar previsões de Analise de Sentimento em Avaliacao de Produtos com Machine Learning (ML).

Este projeto demonstra o uso do Amazon AWS SageMaker Canvas para construir um modelo de aprendizado de máquina para análise de sentimentos de avaliações de produtos. O objetivo é analisar as avaliações de clientes e determinar se eles recomendam os produtos.

## Vídeo de Demonstração
Aqui está um vídeo de demonstração que mostra todo o processo:

[![Análise de Sentimentos em Avaliações de Produtos usando Amazon AWS SageMaker Canvas](https://img.youtube.com/vi/eFMpne_vVa8/0.jpg)](https://www.youtube.com/watch?v=eFMpne_vVa8)


## Índice
1. [Introdução](#introdução)
2. [Conjunto de Dados](#conjunto-de-dados)
3. [Preparação dos Dados](#preparação-dos-dados)
4. [Construção do Modelo](#construção-do-modelo)
5. [Resultados](#resultados)
6. [Uso](#uso)
7. [Conclusão](#conclusão)
8. [Licença](#licença)

### 1. Introdução
Olá, meu nome é Hueini David. Sou formado em Ciências da Computação e atualmente estou cursando Pós-Graduação em Inteligência Artificial e Aprendizagem de Máquina.

Este projeto é uma demonstração prática das habilidades adquiridas no curso "Bootcamp Nexa Machine Learning para Iniciantes" da DIO.

A análise de sentimentos é uma ferramenta poderosa usada para entender opiniões e feedbacks de clientes. 
Este projeto utiliza o Amazon AWS SageMaker Canvas para criar um modelo de aprendizado de máquina que analisa as avaliações de produtos para identificar sentimentos positivos ou negativos e determinar recomendações.

## Conjunto de Dados
O conjunto de dados utilizado neste projeto consiste em avaliações de produtos.

- `BASE COMPLETA`: Base de Dados Completa com todas as colunas e formatos originais da fonte.
- `BASE TRARADA`: Base de Dados Tratada, somente com as colunas necessárias e feito tratamento de texto (Removido caracteres, numeros, acentos, e convertido tudo para minusculo).
- `BASE PARA PREVISAO`: Base de Dados Aleatória criada pelo Gemini para simular analises de Clientes.
- `RESULTADO DAS PREVISOES - BASE COMPLETA`: 19/20.
- `RESULTADO DAS PREVISOES - BASE TRATADA`: 20/20.

### 3. Base de Dados

A base de dados utilizada contém avaliações de clientes sobre diversos produtos. As colunas principais são:
- **Review**: Texto da avaliação do cliente.
- **Recomendação**: Indicação se o cliente recomenda ou não o produto (Sim ou Não).

### 4. Tratamento de Dados

Para melhorar a eficiência do modelo, a base de dados foi tratada da seguinte forma:
- Conversão de texto para minúsculas.
- Remoção de caracteres especiais e números.
- Manutenção apenas das colunas relevantes (review e recomendação).

### 5. Treinamento do Modelo

Utilizamos o Amazon SageMaker Canvas para treinar dois modelos:
- **Modelo com Base Completa**: Inclui todas as colunas, sem tratamento específico.
- **Modelo com Base Tratada**: Inclui apenas as colunas relevantes e dados tratados.

### 6. Resultados

Os resultados mostraram que o modelo treinado com a base tratada teve um desempenho superior, com uma acurácia de 94.74%, comparado aos 93.62% do modelo com base completa. As métricas de avaliação incluíram:
- **Precision**: 99.12%
- **Recall**: 96.9%
- **F1-Score**: Calculado como a média harmônica entre Precision e Recall.

### 7. Análises

Realizamos previsões com o modelo treinado utilizando novas avaliações de produtos. As análises confirmaram que o modelo é capaz de prever corretamente o sentimento das avaliações, com alta precisão para tanto avaliações positivas quanto negativas.

### Exemplo de Dados

Aqui estão as 5 primeiras colunas da base de dados utilizada:

| ClienteID | ProdutoID | Review                                | Recomendação | Data       |
|-----------|------------|---------------------------------------|--------------|------------|
| 1         | 101        | Ótimo produto, recomendo!             | Sim          | 2021-01-01 |
| 2         | 102        | Produto de baixa qualidade.           | Não          | 2021-01-02 |
| 3         | 103        | Chegou no prazo e funciona bem.       | Sim          | 2021-01-03 |
| 4         | 104        | Não gostei, esperava mais.            | Não          | 2021-01-04 |
| 5         | 105        | Excelente, superou minhas expectativas! | Sim          | 2021-01-05 |

## Conclusão

Concluímos com sucesso o projeto de análise de sentimentos utilizando Amazon AWS SageMaker Canvas. O modelo demonstrou alta eficiência na classificação de avaliações de produtos, destacando a importância do tratamento adequado dos dados para obter melhores resultados.
