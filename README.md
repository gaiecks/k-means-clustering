# Segmentação de Clientes com K-means utilizando Python

Este projeto tem como objetivo realizar a segmentação de clientes de um shopping utilizando o algoritmo de clustering K-means. A segmentação permite identificar grupos distintos de clientes com características semelhantes, auxiliando na criação de estratégias de marketing direcionadas e personalizadas.

Foi utilizada a base de dados "Mall Customer Segmentation Data", disponível no link:
[Dataset_Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).

A linguagem utilizada foi Python utilizando o notebook do Google Colab. Para ver o projeto completo basta acessar o link [K-means](https://github.com/gaiecks/k-means-clustering/blob/main/kMeans_Clustering.ipynb).


## Descrição do Projeto

A segmentação de clientes é uma técnica poderosa para entender melhor os diferentes perfis de consumidores e como eles se comportam. Neste projeto, utilizamos dados de clientes de um shopping, focando nas seguintes variáveis:
- Idade
- Renda Anual (em milhares de dólares)
- Pontuação de Gastos (1-100)


## Metodologia

1. **Carregamento dos Dados:**
   - Foi utilizado um dataset de clientes do shopping, contendo informações sobre idade, renda anual e pontuação de gastos.

2. **Pré-processamento:**
   - Verificação de valores ausentes (não há).
   - Seleção das colunas relevantes: `Age`, `Annual Income (k$)` e `Spending Score (1-100)`.
   - Normalização dos dados usando `StandardScaler` para garantir que todas as variáveis estejam na mesma escala.

3. **Determinação do Número Ideal de Clusters:**
   - Foi aplicado o método do cotovelo para determinar o número ótimo de clusters.
   - Após análise do gráfico do cotovelo, foi identificado o ponto onde a diminuição do WCSS começa a se estabilizar, indicando 4 clusters como o número ideal.

4. **Aplicação do K-means:**
   - O algoritmo K-means foi configurado para segmentar os clientes em 4 clusters.

5. **Análise dos Resultados:**
   - As médias das variáveis para cada cluster foram calculadas, permitindo uma interpretação detalhada dos diferentes segmentos de clientes.


## Principais Achados

### Cluster 0: Adultos com Alta Renda e Alta Pontuação de Gastos
- **Idade Média:** 32.88 anos
- **Renda Anual Média:** 86.10 mil dólares
- **Pontuação de Gastos Média:** 81.53
- **Perfil:** Adultos que têm alta renda e alta propensão a gastar. Estratégias de marketing voltadas para produtos premium e exclusivos são recomendadas.

### Cluster 1: Jovens com Renda Baixa e Moderada Pontuação de Gastos
- **Idade Média:** 25.44 anos
- **Renda Anual Média:** 40.00 mil dólares
- **Pontuação de Gastos Média:** 60.30
- **Perfil:** Jovens com renda relativamente baixa, mas com propensão moderada a gastar. Promoções e programas de fidelidade podem atrair este grupo.

### Cluster 2: Adultos com Alta Renda e Baixa Pontuação de Gastos
- **Idade Média:** 39.37 anos
- **Renda Anual Média:** 86.50 mil dólares
- **Pontuação de Gastos Média:** 19.58
- **Perfil:** Adultos com alta renda, mas baixa propensão a gastar. Campanhas destacando o valor e a qualidade dos produtos podem incentivar mais gastos.

### Cluster 3: Clientes Mais Velhos com Renda Média e Baixa Pontuação de Gastos
- **Idade Média:** 53.98 anos
- **Renda Anual Média:** 47.71 mil dólares
- **Pontuação de Gastos Média:** 39.97
- **Perfil:** Clientes mais velhos com renda média e baixa propensão a gastar. Oferecer produtos que agreguem valor e segurança pode ser uma estratégia eficaz.


## Conclusão

A segmentação de clientes utilizando K-means revelou quatro grupos distintos, cada um com características e comportamentos únicos. Essas informações são essenciais para desenvolver estratégias de marketing personalizadas, melhorar a experiência do cliente e aumentar a eficiência das campanhas de marketing.

