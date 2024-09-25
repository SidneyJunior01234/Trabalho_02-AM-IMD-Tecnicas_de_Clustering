# Trabalho_02-AM-IMD-Técnicas_de_Clustering
## Trabalho avaliativo da segunda unidade da disciplina de Aprendizado de Máquina (IMD1101), ofertada pelo Instituto Metrópole Digital (IMD).

A base de dados [Mall Customer Segmentation](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) é disponibilizada no Kaggle por [Vijay Choudhary](https://www.kaggle.com/vjchoudhary7)

O trabalho avaliativo tem como objetivo, aplicar técnicas de clustering (agrupamento) para explorar a base de dados, identificar padrões e tirar conclusões interessantes sobre os dados. Deve-se utilizar diferentes algoritmos de clustering e avaliar o desempenho de cada método.

Foi realizada a aplicação de técnicas de clustering como K-Means, Agrupamento Hierárquico e Agrupamento Espectral visando identificar grupos de clientes com perfis semelhantes.

## Testes iniciais

Inicialmente foi utilizado o K-Means e testado K grupos entre 1 e 9, com essas informações geramos um gráfico em que conseguimos observar com quantos grupos os dados melhor
se comportam. Agrupar em 2, 4 e 8 grupos, mostraram resultados bons e optamos por separar em 2 grupos.

![K Clusters](https://github.com/user-attachments/assets/8083dfa4-8ffa-4816-ae35-f4a08d66b429)

## Resultados

### 1. K-Means

Podemos observar que o K-Means formou dois grupos e a maior concentração dos dados ficou próxima do centroide pertencente ao grupo.

![image](https://github.com/user-attachments/assets/31746582-0b39-405e-82e2-c0b1d3a9842f)

### 2. Agrupamento Hierárquico

Pdemos observar também o Dendograma gerado, que é uma forma de visualizar o agrupamento hierárquico, que há alguns grupos, sendo que a formação de 2 e 4 grupos distintos são mais notáveis.

![image](https://github.com/user-attachments/assets/b8d3780e-979f-4b89-8730-42df835ed91d)

### 1. Agrupamento Espectral

Por último temos a visualização do agrupamento usando o agrupamento espectral. Como o algoritmo utiliza o K-Means para agrupar os dados transformados pelos Autovetores próprios, o resultado tende ser parecido com o K-Means.

![image](https://github.com/user-attachments/assets/3bb3a90b-b4eb-4ed6-9375-cf43e61b568b)

| Modelo | Silhouette | Calinski-Harabasz | Davies-Bouldin |
|---|---|---|---|
| K-means | 0.2776 | 66.9063 | 1.6117 |
| Agrupamento Hierárquico | 0.2418 | 67.0422 | 1.6611 |
| Agrupamento Espectral | 0.2776 | 66.9063 | 1.6117 |

**Tabela 1: Comparação das métricas de avaliação dos algoritmos de agrupamento**

Ao comparar os algoritmos de clustering K-Means, Agrupamento Hierárquico e Agrupamento Espectral para a segmentação de clientes com base em idade, renda anual e pontuação de gastos, observamos que o K-Means e o Agrupamento Espectral apresentaram resultados semelhantes em termos de coesão e separação dos clusters. Ambos os métodos demonstraram clusters bem definidos, enquanto o Agrupamento Hierárquico, embora tenha obtido um Calinski-Harabasz Score ligeiramente superior, mostrou uma coesão e separação dos clusters menos eficazes.

Portanto, para a segmentação eficiente dos clientes nesta base de dados específica, tanto o K-Means quanto o Agrupamento Espectral são escolhas viáveis, com uma leve preferência pelo Agrupamento Espectral devido à sua capacidade de lidar com estruturas complexas nos dados.

## Notebook

[Mall_Customers_Clustering.ipynb](https://github.com/SidneyJunior01234/Trabalho_02-AM-IMD-T-cnicas_de_Clustering/blob/main/Mall_Customers_Clustering.ipynb)

## Realizadores do trabalho avaliativo

[Claudiano Leonardo da Silva](https://github.com/ClaudianoLeonardo)

[Sidney Alves dos Santos Junior](https://github.com/SidneyJunior01234)
