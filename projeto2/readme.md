## Descrição do Problema

### Qual é o problema que você deseja resolver?

Classificação de garrafas defeituosas em uma linha de produção da Coca-Cola. A partir de diferentes imagens de garrafas em uma linha de produção, identificar se existe ou não algum tipo de defeito na garrafa, como a falta da marca, a garrafa estar vazia ou danificada, entre outros.

Serão avaliadas os seguintes quesitos:

* CONTENT_HIGH -> Líquido mais alto que o normal
* CONTENT_LOW -> Líquido mais baixo que o normal
* COVER_NONE -> Sem a tampa 
* BOTTLE_SMASHED -> Garrafa amassada
* LABEL_WHITE -> Rótulo em branco
* LABEL_MISPLACED -> Rótulo errado
* LABEL_NONE -> Rótulo vazio
* BOTTLE_NONE -> Garrafa inexistente


## Base de Dados Utilizada

### Informe a base de dados que será utilizada. Inclua a origem e o link (se aplicável). Informe estatísticas descritivas que considerar relevantes.

A base de dados utilizada será uma versão rotulada da base de dados disponível como material auxiliar do livro "Solomon, C., & Breckon, T. (2010). Fundamentals of Digital Image Processing. Wiley. https://doi.org/10.1002/9780470689776". A base de dados está disponível em https://www.fundipbook.com/materials/ e contém 141 imagens com garrafas que podem conter algum tipo de defeito. Entretanto, temos apenas 77 imagens rotuladas, logo, apenas essas serão utilizadas para avaliação.


## Metas e Critérios de Sucesso

### Escreva como você espera avaliar os resultados e o que considera sucesso mínimo.

Como temos a rotulação correta das 77 imagens, a avaliação será por acurácia e matriz de confusão: quantas falhas ele conseguiu identificar corretamente. Para fins de sucesso mínimo, o algoritmo deverá ser capaz de superar um DummyClassifier, que neste dataset tem uma acurácia de 56%.


## Comentários Adicionais 

Este conjunto de dados e processos foram pensados para serem solucionados com métodos clássicos de processamento digital de imagens, entretanto, neste projeto, buscarei utilizar soluções mais recentes, como CNN, para solucionar o desafio.