# Classificação de Notícias por Assunto

## Identificação
- **Disciplina:** Aprendizagem de Máquina
- **Professor:** Bruno Zolorateff
- **Integrante:** Luan Oliveira

## Descrição do Problema e Objetivo
O projeto aborda a classificação automática de notícias por assunto. O objetivo é treinar um modelo de aprendizagem de máquina que receba o título e a descrição de uma notícia e preveja a categoria mais provável.

Essa solução pode auxiliar na organização de notícias em portais ou sistemas de informação. O modelo será avaliado em notícias que não foram utilizadas durante o treinamento.

## Solução Proposta e Dados
Será utilizado o conjunto de dados AG News, composto por notícias em inglês. As categorias disponíveis são:
- World
- Sports
- Business
- Sci/Tech

O texto de cada notícia será formado pela junção do título e da descrição. Em seguida, o método TF-IDF transformará os textos em vetores numéricos, que serão usados pelo classificador Naive Bayes Multinomial.

**Limitação:** a base está em inglês e não possui uma categoria específica para Política. Portanto, o MVP classificará notícias somente entre as quatro categorias fornecidas.

### Conceitos-Chave
- **TF-IDF (Term Frequency–Inverse Document Frequency):** transforma documentos em representações numéricas, atribuindo pesos aos termos de acordo com sua frequência no texto e na coleção de documentos.
- **Naive Bayes Multinomial:** classificador probabilístico que estima a categoria mais provável para um texto a partir das características extraídas.

## Como Executar
1. Abra o notebook do projeto no Google Colab.
2. Execute as células em ordem, do início ao fim.
3. O notebook instalará, se necessário, a biblioteca para carregar a base de dados.
4. O código carregará e preparará os dados, treinará o modelo e apresentará as métricas de avaliação.
5. Execute a última célula para testar o classificador com uma notícia nova em inglês.

## Resultados
Preencher esta seção após executar o notebook. Usar os valores efetivamente calculados pelo modelo.

- **Acurácia:** [preencher]
- **Precisão macro:** [preencher]
- **Recall macro:** [preencher]
- **F1-score macro:** [preencher]

## Referências
1. Zhang, Xiang; Zhao, Junbo; LeCun, Yann. *Character-level Convolutional Networks for Text Classification*. 2015.
2. Hugging Face Datasets. *AG News — conjunto de dados para classificação de notícias*.
3. Scikit-learn. *Documentação de TfidfVectorizer e MultinomialNB*.
