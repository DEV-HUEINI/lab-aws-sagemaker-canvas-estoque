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

## Introdução
Olá, meu nome é Hueini David. Sou formado em Ciências da Computação e atualmente estou cursando pós-graduação em Inteligência Artificial e Aprendizagem de Máquina. 
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

## Preparação dos Dados
A preparação dos dados é uma etapa crucial na construção de um modelo de aprendizado de máquina eficaz. Foram realizados os seguintes passos:
1. **Upload dos Dados**: O conjunto de dados foi carregado no Amazon S3.
2. **Limpeza dos Dados**: Remoção de colunas e linhas desnecessárias. Apenas as colunas `review` e `recommend` foram mantidas para análise.
3. **Processamento de Texto**: Realização de etapas de pré-processamento de texto, como tokenização, remoção de stop words e stemming/lemmatização.

## Construção do Modelo
Usando o Amazon SageMaker Canvas, foram seguidos os seguintes passos para construir o modelo de análise de sentimentos:
1. **Importação do Conjunto de Dados**: Importação do conjunto de dados limpo do Amazon S3.
2. **Engenharia de Características**: Extração de características dos dados textuais.
3. **Treinamento do Modelo**: Configuração e treinamento do modelo de análise de sentimentos usando o SageMaker Canvas.
4. **Avaliação do Modelo**: Avaliação do desempenho do modelo usando várias métricas como acurácia, precisão, recall e F1-score.

## Resultados
O modelo alcançou as seguintes métricas de desempenho:
- **Acurácia**: `xx%`
- **Precisão**: `xx%`
- **Recall**: `xx%`
- **F1-Score**: `xx%`

## Uso
Para usar este modelo:
1. **Clone o Repositório**: `git clone https://github.com/your-username/sentiment-analysis-aws-sagemaker.git`
2. **Carregue o Conjunto de Dados**: Certifique-se de que seu conjunto de dados esteja carregado no Amazon S3.
3. **Execute o Modelo**: Siga as instruções no repositório para importar o conjunto de dados no SageMaker Canvas e executar o modelo.

## Conclusão
Este projeto demonstra o poder do Amazon AWS SageMaker Canvas na construção de modelos de aprendizado de máquina com o mínimo de codificação. O modelo de análise de sentimentos fornece insights sobre as avaliações dos clientes e ajuda a entender a satisfação do cliente.

## Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
