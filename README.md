# Twitter-Emotion-Classification

PROFESSOR: Tiago Eugenio de Melo

NOMES:
	ÁUREA CRISTIANE RIBEIRO DE LIMA, 
	DANIEL NASCIMENTO MOTTA, 
	MONIQUE SOUSA SILVA, 
	VITOR HUGO DA SILVA LIMA

#Twitter Emotion Classification

Este projeto tem como objetivo classificar emoções expressas em tweets utilizando técnicas de Processamento de Linguagem Natural (PLN) e Redes Neurais com LSTM.

A ideia principal é treinar um modelo que consiga identificar emoções como alegria, raiva, tristeza, medo, entre outras, com base no texto dos tweets.  
Este repositório foi desenvolvido como parte de uma atividade prática da pós-graduação em Ciência de Dados.

---

#Dataset

O dataset utilizado é o [**Emotion Dataset for Emotion Recognition Tasks**](https://www.kaggle.com/datasets/shtrausslearning/emotion-dataset), disponível no Kaggle.

### Principais informações:
- Colunas: `Text`, `Emotion`
- O dataset é balanceado e contém várias classes emocionais
- Formato: `.csv`

##Requisitos

Para executar o projeto localmente, certifique-se de ter o Python 3.7+ e instale os pacotes necessários com:

pip install -r requirements.txt

1. Como Executar
Clone o repositório:

git clone https://github.com/seu-usuario/twitter-emotion-classification.git
cd twitter-emotion-classification

2. Baixe o dataset do Kaggle e coloque o arquivo emotion_dataset.csv na pasta do projeto.

3. Execute o notebook Jupyter:
jupyter notebook twitter_emotion_classification.ipynb

4. Etapas do Projeto
4.1 Importação de bibliotecas: pacotes essenciais para análise de texto e machine learning.

4.2 Carregamento dos dados: leitura e visualização do dataset.

4.3 Pré-processamento:

- Limpeza de texto (remoção de pontuação, links, números)
- Remoção de stopwords
- Lematização com nltk

4.4 Tokenização e Padding: transformação dos textos em sequências numéricas.

4.5 Codificação de rótulos: emoções são convertidas para números com LabelEncoder.

4.6 Construção do modelo LSTM:

- Embedding → LSTM → Dense
- Função de perda: sparse_categorical_crossentropy

4.7 Treinamento e avaliação: divisão em treino/teste e avaliação da acurácia.

5. Resultados
O modelo foi treinado por 10 épocas e obteve uma acurácia satisfatória no conjunto de teste. O desempenho pode ser melhorado utilizando embeddings pré-treinados como GloVe ou BERT.

6. Aprendizados
Este projeto consolidou conhecimentos em:
- Pré-processamento de dados textuais
- Uso de LSTM para classificação
- Avaliação de modelos em PLN
- Tokenização e vetorização de texto


