**Lung Disease Classification using CNN and Transfer Learning**

This project is aimed at classifying the given image of a lung into one of four classes: normal lung, lung affected by COVID-19, viral pneumonia, or bacterial pneumonia. The model is built using transfer learning and the ResNET50 model is used to build the CNN network.

**Dataset**

Two datasets have been used to train and test the model. One dataset is from the COVID-19 Chest X-ray dataset and the other one is from the Chest X-ray Pneumonia dataset. These datasets contain images of lungs of different individuals and the corresponding labels.
Dataset Souce::https://github.com/ieee8023/covid-chestxray-dataset and https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia.

**Approach**

We have used transfer learning to build the CNN network using the ResNET50 model. The model is trained on the above datasets and the accuracy is measured on the test set. We have also implemented early stopping in the code to avoid overfitting.

**Results**

After building the CNN network and testing it on the test set, we found that the accuracy on the test set is 83.33%. The model can classify the elements in a pretty good way.

