# Baita lista de referências de machine learning com foco em visão
 
Esse guia resume um pouco dos meus passos

### Primeiros passos: O que é uma rede neural?
[(Video) 3blue1brown - But what *is* a neural network?](https://www.youtube.com/watch?v=aircAruvnKk) Explica conceitos básicos
de estrutura, operações e treinamento de forma visual/geométrica. Obs: A arquitetura utilizada é o MLP ou Multi Layer 
Perceptron, uma das arquieteturas mais simples para redes neurais.

[(Video-aulas) Coding Train - The Nature of Code - Introduction to Neural Networks](https://www.youtube.com/watch?v=XJ7HLz9VYz0&list=PLRqwX-V7Uu6aCibgK1PTWWu9by6XFdCfh):
Uma approach bem lúdica, explica os conceitos mais básicos de redes neurais em uma sequência de aulas e prática em 
javascript. Inicia com conceitos de baixo nível como perceptron, matrizes e gradientes (inclusive ele escreve a 
própria lib de operações com matrizes, mas pode pular essa parte) e termina escrevendo uma rede neural que joga uma
versão simplificada de flappy bird. Acompanha o livro dele [Nature of Code](https://natureofcode.com/), capítulo 10.
Também utiliza MLP para explicar os conceitos gerais que podem ser aplicados a outras arquiteturas mais complexas.

### Level Up: Convoluções para redes neurais
Apesar de muito poderosas, as técnicas de ML como são as redes MLP tem algumas limitações quando aplicadas a imagens. 
A quantidade de parâmetros (weights e biases) cresce exponencialmente de acordo com a resolução da imagem de entrada, 
o que requer muito hardware para rodar modelos mais complexos. O conceito de convoluções entra na jogada nesse contexto.

[(Video) Computerphile - How Blurs and Filters Work?](https://www.youtube.com/watch?v=C_zFhWdM4ic) O que é um "filtro" e como
funciona uma convolução no contexto de visão computacional?

[(Video) Computerphile - Finding the Edges (Sobel Operator)](https://www.youtube.com/watch?v=uihBwtPIBxM) Bom exemplo de aplicação
de filtros e convoluções em visão clássica. *Assista pensando em o que acontece quando podemos variar os valores do filtro
em si!*

[(Video) Computerphile - Neural Network that Changes Everything](https://www.youtube.com/watch?v=py5byOOHZM8) Faz o link da aplicação
de convoluções na visão clássica com seu uso em redes neurais convolucionais (Adivinha da onde vem esse nome?)

[(Blog Post) Towards Data Science - Intuitively Understanding Convolutions for Deep Learning](https://towardsdatascience.com/intuitively-understanding-convolutions-for-deep-learning-1f6f42faee1)
Finalmente um pouco de texto! Os conceitos anteriores são resumidos nesse post, é uma boa referência (com animações!)
pra internalizar o funcionamento de filtros e alguns de seus parâmetros já com o contexto de deep learning em mente.

### Deep learning: Histórico, tipos de modelos e mão na massa!

[(Blog Post) Towards Data Science - AlexNet: The Architecture that Challenged CNNs](https://towardsdatascience.com/alexnet-the-architecture-that-challenged-cnns-e406d5297951)
Considerado o pontapé da recente revolução das CNNs, esse [paper](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)
de 2012 possibilitou a aplicação de redes neurais convolucionais a grandes datasets de imagens de alta resolução

[(Blog Post) Analytics Vidhya - Image Classification vs. Object Detection vs. Image Segmentation](https://medium.com/analytics-vidhya/image-classification-vs-object-detection-vs-image-segmentation-f36db85fe81)
Resumo bem curto diferenciando classificação, detecção de objetos e segmentação, os três grandes grupos de ML com imagens

[(Blog Post) Towards Data Science - Detection and Segmentation through ConvNets](https://towardsdatascience.com/detection-and-segmentation-through-convnets-47aa42de27ea)
Revisão mais aprofundada do funcionamento e diferenciação desses três grupos.

[(Tutorial) PyImageSearch - Transfer Learning with Keras and Deep Learning](https://www.pyimagesearch.com/2019/05/20/transfer-learning-with-keras-and-deep-learning/)
Mão na massa! Essa série utiliza o Keras para treinar um classificador simples usando Keras. Esse primeiro post utiliza
a CNN como **feature extractor** ou seja, um módulo de reconhecimento de padrões, e realiza a classificação com modelos
de machine learning tradicionais (SVM e Logistic Regression)

[(Tutorial) PyImageSearch - Fine-tuning with Keras and Deep Learning](https://www.pyimagesearch.com/2019/06/03/fine-tuning-with-keras-and-deep-learning/)
Segundo post com tutorial para utilização do Keras. Dessa vez, usando uma rede neural como "Head" do modelo ao invés da regressão.

#[WIP]
Vem mais por aí!