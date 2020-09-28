# laba2

Суть второй лабораторной работы: попытаться обучить нейросеть с различными начальными параметрами:

Число слоев
Количество нейронов на слоях
Шаг обучения Batch_size = 256, epoch = 200.
Исходная нейросеть

    tf.keras.layers.Input(shape=(224,224,3)),
    tf.keras.layers.Conv2D(filters=8, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=8, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)
    
Image alt

![Image alt]()

Нейросеть 2
Добавляем 1 полносвязный слой (filters=8, kernel_size=3)

    tf.keras.layers.Input(shape=(224,224,3)),
    tf.keras.layers.Conv2D(filters=8, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=8, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=8, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)
Image alt

Нейросеть 3
В слоях меняем (filters=8, kernel_size=3) на (filters=16, kernel_size=3)

    tf.keras.layers.Input(shape=(224,224,3)),
    tf.keras.layers.Conv2D(filters=16, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=16, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=16, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)
Image alt

Нейросеть 4
В слоях меняем (filters=16, kernel_size=3) на (filters=32, kernel_size=3)

    tf.keras.layers.Input(shape=(224,224,3)),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)
    
Нейросеть 5
Добавляем 1 полносвязный слой (filters=32, kernel_size=3)

    tf.keras.layers.Input(shape=(224,224,3)),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Conv2D(filters=32, kernel_size=3),
    tf.keras.layers.MaxPool2D(),
    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)
Image alt
