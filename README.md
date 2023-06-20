# Convolutional_Neural_Network-Univali

Trabalho de estudos designados pelo tutor Felipe Viel
Classificação de Imagens com CNN no conjunto de dados CIFAR-10

Este repositório contém um código exemplo em Python retirado dos modelos disponibilizados pelo Tensorflow e Keras que implementa uma Rede Neural Convolucional (CNN) para a classificação de imagens no conjunto de dados CIFAR-10.

## Conjunto de dados CIFAR-10

O conjunto de dados CIFAR-10 consiste em 60.000 imagens coloridas de 32x32 pixels, divididas em 10 classes diferentes. Cada classe contém 6.000 imagens. As classes incluem objetos como avião, automóvel, pássaro, gato, cervo, cachorro, sapo, cavalo, navio e caminhão.

## Funcionalidade do código

O código implementa a estrutura da CNN utilizando a biblioteca TensorFlow e Keras. Ele define camadas convolucionais, camadas de pooling e camadas densas para realizar a classificação das imagens. A função de ativação utilizada é a ReLU (Rectified Linear Unit).

A implementação também realiza a normalização dos valores de pixel das imagens para o intervalo entre 0 e 1. Em seguida, ele divide o conjunto de dados em conjuntos de treinamento e teste.

Durante o treinamento da CNN, o modelo é alimentado com as imagens do conjunto de treinamento e suas respectivas classes. Através da técnica de aprendizado supervisionado, o modelo ajusta os pesos das camadas para minimizar a função de perda (no caso, a entropia cruzada) e melhorar sua capacidade de fazer previsões precisas.

O treinamento é realizado por várias fases, onde cada fases envolve o processamento de todo o conjunto de treinamento. Após cada fase, o modelo é avaliado usando o conjunto de validação (conjunto de dados não utilizado durante o treinamento) para monitorar o desempenho e evitar o overfitting (sobreajuste). Isso permite avaliar a capacidade do modelo de fazer previsões precisas em dados não vistos anteriormente.

## Utilização

Para executar o código, é necessário ter as bibliotecas TensorFlow, Keras, NumPy e Matplotlib instaladas. O conjunto de dados CIFAR-10 é carregado automaticamente pela função datasets.cifar10.load_data() da biblioteca Keras.

Após a execução do código, é possível visualizar as imagens do conjunto de treinamento e a respectiva classe abaixo de cada imagem. Também é possível visualizar uma imagem do conjunto de teste juntamente com a classe prevista pelo modelo.

## Resultados

O modelo treinado alcançou uma precisão de 74% no conjunto de teste, demonstrando sua capacidade de classificar corretamente as imagens do conjunto CIFAR-10.
Agradecimentos

## Referências

 - Documentação oficial do TensorFlow: https://www.tensorflow.org/
 - Documentação oficial do Keras: https://keras.io/
 - Página do conjunto de dados CIFAR-10: https://www.cs.toronto.edu

### Gostaria de expressar meus sinceros agradecimentos ao tutor Felipe Viel por sua orientação e suporte durante o desenvolvimento deste trabalho acadêmico.
