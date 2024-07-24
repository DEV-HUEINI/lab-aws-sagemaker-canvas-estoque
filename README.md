# 📊 Análise de Sentimentos em Avaliações de Produtos usando Amazon AWS [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Neste Projeto para o Curso de IA do Lab DIO, usei o SageMaker Canvas para criar previsões de Analise de Sentimento em Avaliacao de Produtos com Machine Learning (ML).

Este projeto demonstra o uso do Amazon AWS SageMaker Canvas para construir um modelo de aprendizado de máquina para análise de sentimentos de avaliações de produtos. O objetivo é analisar as avaliações de clientes e determinar se eles recomendam os produtos.

## Vídeo de Demonstração
Aqui está um vídeo de demonstração que mostra todo o processo:

[![Análise de Sentimentos em Avaliações de Produtos usando Amazon AWS SageMaker Canvas](https://img.youtube.com/vi/eFMpne_vVa8/0.jpg)](https://www.youtube.com/watch?v=eFMpne_vVa8)


![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

## Índice
- [Introdução](#introdução)
- [Conjunto de Dados](#conjunto-de-dados)
- [Preparação dos Dados](#preparação-dos-dados)
- [Construção do Modelo](#construção-do-modelo)
- [Resultados](#resultados)
- [Uso](#uso)
- [Conclusão](#conclusão)
- [Licença](#licença)

## Introdução
A análise de sentimentos é uma ferramenta poderosa usada para entender opiniões e feedbacks de clientes. Este projeto utiliza o Amazon AWS SageMaker Canvas para criar um modelo de aprendizado de máquina que analisa as avaliações de produtos para identificar sentimentos positivos ou negativos e determinar recomendações.

## Conjunto de Dados
O conjunto de dados utilizado neste projeto consiste em avaliações de produtos. Inclui as seguintes colunas:
- `review`: O texto da avaliação do cliente.
- `recommend`: Um indicador binário de se o cliente recomenda o produto (1 para recomendar, 0 para não recomendar).

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
