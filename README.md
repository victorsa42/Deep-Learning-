# Deep-Learning- Projeto de sensores inteligentes para IOT

Aplicações de Redes de Deep Learning em Sensores Inteligentes

Neste projeto o objetivo é implementar/otimizar uma rede de Deep Learning para reconhecimento de imagens digitais. Por meio dos conteúdos apresentados em aulas, deve ser possível otimizar os parâmetros de uma rede neural para reconhecer imagens digitais.

O modelo de arquitetura proposta e essa, mas você pode otimizar da forma que achar necessário:

model = tf.keras.models.Sequential([

tf.keras.layers.Conv2D(32, (3,3), activation='relu', input_shape=(150, 150, 3)),

tf.keras.layers.MaxPooling2D(2, 2),

tf.keras.layers.Conv2D(64, (3,3), activation='relu'),

tf.keras.layers.MaxPooling2D(2,2),

tf.keras.layers.Conv2D(128, (3,3), activation='relu'),

tf.keras.layers.MaxPooling2D(2,2),

tf.keras.layers.Conv2D(128, (3,3), activation='relu'),

tf.keras.layers.MaxPooling2D(2,2),

tf.keras.layers.Flatten(),

tf.keras.layers.Dense(512, activation='relu'),

tf.keras.layers.Dense(2)

])

É possível ter acesso também a esse modelo no ambiente COLAB: (https://colab.research.google.com/github/tensorflow/examples/blob/master/courses/udacity_intro_to_tensorflow_for_deep_learning/l05c01_dogs_vs_cats_without_augmentation.ipynb#scrollTo=F15-uwLPVrWa).

O principal objetivo do projeto é aplicar a técnica de Transfer Learning para novos objetos a serem classificados na rede. Neste exemplo, usamos gatos e cachorros, mas você pode usar outros exemplos, como: você e sua esposa, pessoas famosas, reconhecer notas de dinheiro, reconhecer os gestos da linguagem de libras, frutos verdes e maduros, dentre outras situações.
