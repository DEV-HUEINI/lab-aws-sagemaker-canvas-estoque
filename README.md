
## Análise de Sentimentos em Avaliações de Produtos usando Amazon AWS [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Olá, meu nome é Hueini David. 

Sou formado em Ciências da Computação e atualmente estou cursando Pós-Graduação em Inteligência Artificial e Aprendizagem de Máquina.

Este projeto é uma demonstração prática das habilidades adquiridas no curso "Bootcamp Nexa - Machine Learning para Iniciantes na AWS" da DIO em parceria com a Amazon AWS.


## Vídeo do Projeto
Aqui está um vídeo de demonstração que mostra todo o processo:

[![Análise de Sentimentos em Avaliações de Produtos usando Amazon AWS SageMaker Canvas](https://img.youtube.com/vi/eFMpne_vVa8/0.jpg)](https://www.youtube.com/watch?v=eFMpne_vVa8)

##
<details open>
  <summary><h2>Índice</h2></summary>
  <table>
    <tr>
      <td>1.</td>
      <td><a href="#1-introdução">Introdução</a></td>
    </tr>
    <tr>
      <td>2.</td>
      <td><a href="#2-base-de-dados">Base de Dados</a></td>
    </tr>
    <tr>
      <td>3.</td>
      <td><a href="#3-tratamento-de-dados">Tratamento de Dados</a></td>
    </tr>
    <tr>
      <td>4.</td>
      <td><a href="#4-treinamento-do-modelo">Treinamento do Modelo</a></td>
    </tr>
    <tr>
      <td>5.</td>
      <td><a href="#5-resultados-e-métricas">Resultados e Métricas</a></td>
    </tr>
    <tr>
      <td>6.</td>
      <td><a href="#6-análise">Análises</a></td>
    </tr>
    <tr>
      <td>7.</td>
      <td><a href="#7-conclusão">Conclusão</a></td>
    </tr>
  </table>
</details>

##
## 1. Introdução
A análise de sentimentos é uma ferramenta poderosa usada para entender opiniões e feedbacks de clientes. 
Este projeto utiliza o Amazon AWS SageMaker Canvas para criar um modelo de aprendizado de máquina que analisa as avaliações de produtos para identificar sentimentos positivos ou negativos e determinar recomendações.

## 2. Base de Dados

A base de dados utilizada contém avaliações de clientes sobre diversos produtos. As colunas principais são:
- **`Review`**: Texto da avaliação do cliente.
- **`Recomendação`**: Indicação se o cliente recomenda ou não o produto (Sim ou Não).

| Date       | Review                | Overall Rating | Recommend to a Friend |
|------------|------------------------|----------------|------------------------|
| 2024-07-01 | Excelente produto!    | 5              | Sim                    |
| 2024-07-02 | Muito bom, mas pode melhorar | 4              | Não                    |
| 2024-07-03 | Não gostei do produto | 2              | Não                    |




## 3. Tratamento de Dados

Para melhorar a eficiência do modelo, a base de dados foi tratada da seguinte forma:
- Conversão de texto para minúsculas.
- Remoção de caracteres especiais e números.
- Manutenção apenas das colunas relevantes (review e recomendação).

## 4. Treinamento do Modelo

Utilizamos o Amazon SageMaker Canvas para treinar dois modelos:
- **Modelo com Base Completa**: Inclui todas as colunas, sem tratamento específico.
![image](https://github.com/user-attachments/assets/beaac05b-d6e3-459c-9649-952e54a4506a)

- **Modelo com Base Tratada**: Inclui apenas as colunas relevantes e dados pré-processados.
![image](https://github.com/user-attachments/assets/aeed1bf7-e4b0-4e46-9530-6d724a6466e8)


## 5. Resultados e Métricas

Os resultados mostraram que o modelo treinado com a base tratada teve um desempenho superior comparado ao modelo com base completa. As métricas de avaliação incluíram:

![image](https://github.com/user-attachments/assets/68c88905-12c1-4ea0-a7c5-eae928afcf4b)
![image](https://github.com/user-attachments/assets/c7bf6079-4df0-4b8e-a0c4-c9719be424ed)

<p>
  <img src="https://github.com/user-attachments/assets/3f98b212-9e1d-428b-bda2-3598948a3b70" alt="Gráfico de Performance do Modelo" width="500" style="display: inline-block; border: 2px solid #ddd; padding: 5px; margin: 10px; box-sizing: border-box;"/>
  <img src="https://github.com/user-attachments/assets/b9781648-0461-4729-b56b-6a7670e61c06" alt="Matriz de Confusão" width="500" style="display: inline-block; border: 2px solid #ddd; padding: 5px; margin: 10px; box-sizing: border-box;"/>
</p>

<h3>Calculo de Métricas</h3>

- **Recall (Sensibilidade)**: Capacidade do modelo de identificar todos os valores reais.  
`Recall = TP / (TP + FN)`

- **Precisão**: Capacidade das previsões do modelo estarem corretas.  
`Precisão = TP / (TP + FP)`

- **Acurácia**: Proporção de previsões corretas tanto para SIM quanto para NÃO.  
`Acurácia = (TP + TN) / Total de Previsões`

- **F1-Score**: Média harmônica entre Recall e Precisão.  
`F1-Score = 2 * (Precisão * Recall) / (Precisão + Recall)`

## 6. Análise

Realizamos previsões com o modelo treinado utilizando novas avaliações de produtos. As análises confirmaram que o modelo é capaz de prever corretamente o sentimento das avaliações, com alta precisão para tanto avaliações positivas quanto negativas.

![image](https://github.com/user-attachments/assets/e5f1af53-6367-4aff-bc64-b2c778887491)

## 7. Conclusão

Concluímos com sucesso o projeto de análise de sentimentos utilizando Amazon AWS SageMaker Canvas. O modelo demonstrou alta eficiência na classificação de avaliações de produtos, destacando a importância do tratamento (pré-processamento) adequado dos dados para obter melhores resultados.
