# Atividade Prática com Gephi e Wikipedia

Este projeto tem como objetivo a construção e visualização de uma rede semântica a partir de artigos da Wikipédia relacionados ao termo Artificial Neural Network.

## Descrição da Atividade
Utilizamos a biblioteca wikipedia para coletar páginas a partir de um termo semente (Artificial Neural Network) e seguimos os links internos entre os artigos para formar uma rede de conhecimento. A coleta foi realizada de forma limitada a duas camadas de profundidade, com a remoção de palavras irrelevantes por meio de uma lista customizada de stopwords.

## Filtragem de conteúdo
Para garantir que a rede gerada represente conexões relevantes, foi aplicada uma filtragem manual com base em termos genéricos e técnicos comuns da Wikipédia, como:

Termos genéricos de ciência e computação (data, system, method, model, learning, etc.)

Termos específicos da Wikipédia (category, article, citation, reference, etc.)

Identificadores e códigos de publicações científicas (DOI, ISBN, PMID, etc.)

Esses termos foram excluídos da rede para evitar conexões espúrias e melhorar a análise.

## Dados da Rede
Total inicial: 70.895 nós e 205.505 arestas

Subgrafo extraído com grau mínimo > 24:
1.027 nós e 58.285 arestas

Este subgrafo foi exportado em formato .graphml e visualizado no Gephi.

## Visualização (Gephi)
Utilizou-se o Gephi 0.10.1 para:

Visualizar a topologia da rede com layout ForceAtlas2

Colorir comunidades detectadas via modularidade

Redimensionar os nós com base no grau

Aplicar rotação e filtros visuais para melhor análise

##Observações

O projeto demonstra como explorar automaticamente conexões conceituais a partir da Wikipédia.

Ideal para introdução a análise de redes complexas, ciência de dados e visualização com Gephi.
