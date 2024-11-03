# ekg-classify-ai

The [Kaggle ECG Heartbeat Categorization Dataset](https://www.kaggle.com/datasets/shayanfazeli/heartbeat/data) is used to classify pre-processed and segmented ECG signals into 5 classes:  Normal, Supraventricular Ectopy, Ventricular Ectopy, Fusion, and Unknown Beats. Typical, random signals from the training and testing data set are shown below.
![image](https://github.com/user-attachments/assets/d17705e3-f84b-4367-bbca-8260990497f2)
![image](https://github.com/user-attachments/assets/23ba4c27-5020-4195-8de5-4f246a646dd0)

The distribution of classes in the testing data set is shown below.
![image](https://github.com/user-attachments/assets/0e0db666-3212-420e-b968-b2ded9c525ea)

A [convolutional neural network](https://en.wikipedia.org/wiki/Convolutional_neural_network) or CNN was used with 5 layers. Each layer was composed of a convolutional operation, maxpooling, and ReLU activation with a final dense network to recover the predicted label. The model is reduces error by minimizing a [cross-entropy](https://en.wikipedia.org/wiki/Cross-entropy) loss function as shown below.
![image](https://github.com/user-attachments/assets/fa89b770-84e3-4307-bdbe-75009d1796f7)
![image](https://github.com/user-attachments/assets/518c49fc-067f-43d5-b8ee-eed471981feb)

At the end, the model is able to predict classes with an overall accuracy of 90.49% as shown below.
![image](https://github.com/user-attachments/assets/a01877ca-6ab3-4580-bb75-2ca07d938b7e)
