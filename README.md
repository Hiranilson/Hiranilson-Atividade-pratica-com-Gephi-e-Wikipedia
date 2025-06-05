# 🌐 Atividade Prática com Gephi e Wikipedia
Este projeto tem como objetivo a construção e visualização de uma rede semântica a partir de artigos da Wikipédia relacionados ao termo Artificial Neural Network.

## 🧠 Descrição da Atividade
Utilizou-se a biblioteca wikipedia em Python para coletar páginas a partir de um termo semente (Artificial Neural Network). A partir desse ponto, percorremos links internos entre artigos da Wikipédia, formando uma rede conceitual com até duas camadas de profundidade.

Para garantir relevância semântica, foi aplicada uma lista customizada de stopwords, removendo termos excessivamente genéricos ou técnicos.

## 🧹 Filtragem de Conteúdo
A filtragem manual removeu termos que poderiam gerar conexões espúrias, incluindo:

Termos genéricos de ciência e computação: data, system, method, model, learning, etc.

Termos específicos da Wikipédia: category, article, citation, reference, etc.

Identificadores de publicações científicas: DOI, ISBN, PMID, entre outros.

Essa filtragem visou enriquecer a análise da rede, priorizando conexões conceituais relevantes.

## 📈 Dados da Rede
Rede original: 70.895 nós e 205.505 arestas

Subgrafo extraído (grau mínimo > 24):
→ 1.027 nós
→ 58.285 arestas

Este subgrafo foi exportado no formato .graphml e posteriormente visualizado no Gephi.

## 🎨 Visualização com Gephi
A análise visual foi realizada com o Gephi 0.10.1, aplicando os seguintes procedimentos:

Layout: Circle Pack Layout (agrupamento hierárquico em círculos)

Cores: Comunidades detectadas via algoritmo de modularidade

Tamanho dos nós: Proporcional ao grau (número de conexões)

Ajustes visuais: Filtros e rotação para realçar a estrutura da rede

Essa visualização destaca agrupamentos conceituais e estruturas hierárquicas entre os tópicos relacionados.

## 📌 Observações
A atividade demonstra como construir e explorar uma rede semântica automatizada a partir de artigos da Wikipédia.

É uma excelente introdução prática à análise de redes complexas, ciência de dados e visualização com Gephi.
