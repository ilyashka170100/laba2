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

![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_1_2.png)
![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_1_1.png)

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

![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_2_2.png)
![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_2_1.png)

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


![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_3_2.png)
![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_3_1.png)


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
    
    
![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_4_2.png)
![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_4_1.png)
   
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

![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_5_2.png)
![Image alt](https://github.com/ilyashka170100/laba2/blob/master/%D0%BB%D0%B0%D0%B1%D0%B01_5_1.png)

