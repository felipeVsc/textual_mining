## Descrição do Problema

### Qual é o problema que você deseja resolver?

Esse projeto envolve a persona de um jornalista, que está no processo de escrever uma notícia. Ele precisa de ajuda para classificar a sua notícia em diferentes tópicos (ex. política, economia e outros), além de precisar gerar títulos que sejam impactantes e resumos que agreguem a informação mais relevante. 

Esse projeto envolve a automação dessas atividades. O foco principal dele será em **classificar notícias em categorias pré-definidas**. Porém, ele também deverá gerar algumas outras informações relevantes como: *título da noticia; resumo da notícia; palavras-chaves*.

Ou seja, a partir de um texto dado, o ambiente deverá ser capaz de fornecer:

* Categorias daquele texto
* Título
* Resumo
* Palavras-chaves


## Base de Dados Utilizada

### Informe a base de dados que será utilizada. Inclua a origem e o link (se aplicável). Informe estatísticas descritivas que considerar relevantes.


O dataset que será utilizado para este trabalho é o dataset "News Category Dataset", disponível no Kaggle: https://www.kaggle.com/datasets/rmisra/news-category-dataset
 
O dataset contém 210 mil notícias entre 2012 e 2022, retiradas do HuffPost, um tradicional agrupador de sites baseado nos Estados Unidos. Ele contém dados de notícias de mais de 42 categorias, sendo algumas delas: política; bem estar; viagens; estilo e beleza, entre outros. 

Ele é composto dos seguintes atributos:

* category: categoria em que a notícia foi publicada.
* headline: título da notícia.
* authors: lista de autores.
* link: link para a notícia original.
* short_description: resumo da notícia.
* date: data de publicação.

Existem alguns detalhes deste dataset, como o fato de que existem cerca de 10 mil notícias entre 2018 e 2022, mas 200 mil entre 2012 e 2018. Porém, como não iremos tratar do aspecto temporal neste projeto, esse fato não deverá influenciar nos resultados. 


Citação: Misra, Rishabh. "News Category Dataset." arXiv preprint arXiv:2209.11429 (2022).

## Metas e Critérios de Sucesso

A etapa de classificação das categorias deverá ter uma taxa de acurácia acima de X. Esse valor é o valor que um DummyClassifier teria nesta atividade.

Para as atividades de resumo (geração de título, geração de resumos) serão utilizadas métricas de distância em conjuntos com datasets de treino e de teste para avaliar quão próximos os textos gerados pela inteligência artificial estão dos produzidos por jornalistas.

### Escreva como você espera avaliar os resultados e o que considera sucesso mínimo.

A etapa de classificação das categorias deverá ter uma taxa de acurácia acima de X. Esse valor é o valor que um DummyClassifier teria nesta atividade.

Para as atividades de resumo (geração de título, geração de resumos) serão utilizadas métricas de distância em conjuntos com datasets de treino e de teste para avaliar quão próximos os textos gerados pela inteligência artificial estão dos produzidos por jornalistas.




## Comentários Adicionais 

A ideia desse projeto não era apenas fazer uma tarefa de classificação, mas por ter a oportunidade de realizar uma demo, também trazer coisas que possam ser aplicadas a um contexto real, que possam facilitar a vida de alguém.