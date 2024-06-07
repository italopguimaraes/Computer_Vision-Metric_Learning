# Reconhecimento Facial Com Facenet Pytorch Para Aprendizado De Métrica

## Introdução ao Projeto

Um dos desafios do século XXI, no campo do Machine Learning, foi desenvolver modelos de reconhecimento
facial que funcionassem para uma grande variedade de pessoas. Originalmente, podemos pensar que cada
pessoa fosse um indivíduo único, sendo assim uma classe. Logo, os primeiros modelos foram baseados em
modelos de classificação.
Contudo, havia um grande incoveniente nesse processo: toda vez que uma pessoa nova surgia para ser
cadastrada no banco de dados, era necessário treinar o modelo novamente, uma vez que você incluiu uma nova
classe no seu problema. Antes haviam N classes, com a introdução de uma nova pessoa N + 1. Conforme o
sistema fosse aumentando, acabava complicando o procedimento para colocar o sistema em produção
novamente. Uma saída para esse problema, que acabou virando um campo específico de Deep Learning, é o
Aprendizado de Métrica, no inglês Metric Learning. O método consiste em, invés de trabalharmos com um
problema de classificação, treinamos o modelo para aprender uma métrica de distância entre duas entidades. A
saída de um modelo que foi treinado mediante o método de Metric Learning é um vetor descritor. Esse vetor é
responsável por computar as características, ou features, que descrevem a face de uma pessoa. O método de
Metric Learning tornou-se promissor, possibilitando a inclusão de novas pessoas no banco de dados, de forma
que não fosse necessário re-treinar o modelo.
Contudo, apesar de todos nós possuímos características únicas em nossas faces, a pandemia do
Covid-19 trouxe um grande problema para os modelos de reconhecimento facial, as máscaras faciais. Cobrindo
parte importante do nosso rosto, do qual os modelos de deep learning extraíam características para computar
o vetor descritor. Com isso, os modelos de reconhecimento facial apresentavam um alto índice de falhas.
Algumas soluções foram encontradas para contornar esse problema.
Nesse tarefa, você precisará fazer o seguinte:
1) Treinar um modelo de rede neural nesse conjunto de dados.
a. O conjunto de dados possui uma grande variedade de celebridades.
2) Uma vez treinado o modelo, você deve criar um banco de dados com as imagens das
celebridades com o output do vetor descritor do seu modelo.
3) Após o treinamento da rede neural você deve incluir essa pessoa no banco de dados.
4) Uma vez concluídas as etapas (1), (2) e (3), você deve usar esta imagem, que é a pessoa do
item (3) usando máscara facial, e fazer o reconhecimento facial dela.
OBSERVAÇÕES
- Caso você tenha problemas em usar a GPU do Colab, pode utilizar uma rede pré-treinada para criar o
vetor descritor de características dos rostos.
- É obrigatório exibir a imagem que será usada para inferência, isto é, a imagem do item (4), e exibir
qual é o score da métrica que você usará e, também, qual foi a pessoa com a qual ela foi identificada no
banco de dados.
- Caso você nunca tenha trabalhado com metric learning, aqui está um post detalhado sobre o assunto.
LINK.
- Para atingir a pontuação completa da questão, é importante que seu algoritmo consiga fazer o
reconhecimento da pessoa do item 4

## Começando

## Starting

### Google Colab Notebook:
1) Salve uma cópia no google drive do notebook, à partir da url abaixo, e execute as células do notebook sequencialmente preferencialmente na gpu:

https://colab.research.google.com/drive/1f-GXO_XrH0MJ5sH8XxFmRsd9Ol2aiPjy?usp=sharing

2) Coloque os Arquivos 'best_model.pth' e 'celebrities.db' dentro do diretório 'content/'

3) Execute as Celulas Abaixo Sequindo as Instruções Deste Notebook, Preferencialmente na Gpu:

### Executar Localmente

1) Clone o Repositório, em Algum Local da Sua Máquina, Executando o Comando via Git:
git clone https://github.com/italopguimaraes/Computer_Vision-Metric_Learning.git

2) Com o Terminal Entre no Diretório Computer_Vision-Metric_Learning/ e Execute o Comando: jupyter notebook

3) Clique no Arquivo 'Prova_Daedalus_Questao_02.ipynb' e Abra no Navegador, Execute as Células Abaixo Sequindo as Instruções Deste Notebook.