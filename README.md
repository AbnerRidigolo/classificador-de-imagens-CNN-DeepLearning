# Classificador de Imagens CIFAR-10 com CNN em TensorFlow/Keras

## Visão Geral do Projeto

Este projeto de portfólio demonstra a criação de um classificador de
imagens para o dataset CIFAR-10 usando uma Rede Neural Convolucional
(CNN) construída com as bibliotecas TensorFlow e Keras. O objetivo é
desenvolver um modelo capaz de identificar e categorizar imagens em uma
das 10 classes pré-definidas (avião, automóvel, pássaro, gato, veado,
cachorro, sapo, cavalo, navio e caminhão).

O projeto segue uma metodologia profissional, cobrindo o ciclo completo
de um projeto de deep learning, desde o pré-processamento de dados até a
avaliação detalhada do modelo.

## O Problema e sua Relevância

A classificação de imagens é um problema central em visão computacional
com inúmeras aplicações práticas. Este projeto serve como uma introdução
robusta a essa área, permitindo a exploração de técnicas essenciais como
o pré-processamento de dados de imagem, a construção de arquiteturas de
redes neurais convolucionais (CNNs) e o uso de aumento de dados (Data
Augmentation) para melhorar a generalização do modelo.

Ao resolver este problema, o projeto demonstra:

-   Capacidade de aplicar conceitos de Deep Learning para tarefas de
    visão computacional.
-   Habilidade de lidar com dados de imagem complexos.
-   Proficiência na utilização de frameworks como TensorFlow e Keras.

## Ferramentas e Dados

**Dataset**: O projeto utiliza o dataset CIFAR-10, composto por 60.000
imagens coloridas de 32x32 pixels, divididas em 10 classes.

**Frameworks e Bibliotecas**: - TensorFlow/Keras: Utilizado para a
construção, compilação, treinamento e avaliação do modelo. - NumPy: Para
operações eficientes com arrays numéricos. - Matplotlib: Para a
visualização dos dados e resultados, como a matriz de confusão. -
Scikit-learn: Para a geração de um relatório de classificação detalhado.

## Estrutura do Código e Metodologia

### Preparação e Exploração dos Dados:

-   Carregamento do dataset CIFAR-10 diretamente da API do Keras.
-   Pré-processamento dos dados, incluindo a normalização dos valores
    dos pixels para o intervalo \[0, 1\] e a conversão dos rótulos para
    o formato one-hot-encoding.
-   Geração de dados sintéticos através de Data Augmentation (aumento de
    dados) para evitar o overfitting e melhorar a capacidade de
    generalização do modelo.

### Construção da Arquitetura do Modelo:

-   O modelo é uma Rede Neural Convolucional (CNN) sequencial.
-   A arquitetura consiste em múltiplos blocos de camadas convolucionais
    (Conv2D) e de pooling (MaxPooling2D) para extrair e comprimir as
    características visuais das imagens.
-   Camadas de Dropout são adicionadas para regularização, mitigando o
    overfitting.
-   A rede é finalizada com camadas densas (Dense), sendo a camada de
    saída com 10 neurônios e a função de ativação softmax para a
    classificação.

### Treinamento e Avaliação:

-   O modelo é compilado com o otimizador Adam e a função de perda
    categorical_crossentropy.
-   O treinamento é realizado por 20 épocas, utilizando o gerador de
    aumento de dados.
-   A performance do modelo é avaliada no conjunto de teste para obter a
    acurácia final.

## Destaques do Projeto para Recrutadores

Este projeto vai além de uma simples implementação de um modelo. Ele
demonstra habilidades e conhecimentos cruciais para o mercado de
trabalho:

-   **Pensamento Crítico**: A inclusão de Data Augmentation mostra que o
    desenvolvedor entende e pode aplicar técnicas para resolver desafios
    comuns como o overfitting.
-   **Análise Profunda**: A avaliação do modelo não se limita à
    acurácia. A inclusão de um relatório de classificação detalhado (com
    precisão, recall e f1-score por classe) e uma matriz de confusão
    demonstra a capacidade de diagnosticar onde o modelo acerta e erra,
    e de traduzir métricas técnicas em insights práticos.
-   **Comunicação**: A clareza do código e a apresentação dos resultados
    (como a visualização de predições) evidenciam a capacidade de
    comunicar o trabalho de forma eficaz.

## Como Rodar o Projeto

Este projeto pode ser executado facilmente no Google Colaboratory. Siga
estes passos:

1.  Abra um novo notebook no Google Colab.
2.  Copie e cole o código do arquivo `main.py` no notebook.
3.  Execute as células. As bibliotecas necessárias já estão
    pré-instaladas no ambiente do Colab.
