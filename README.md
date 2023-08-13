# Transfer_learning
Multiclass image classification using resent50 to classify pipelines into corroded, cracked, healthy pipelines (custom data set)
training set: 4662 validated image filenames belonging to 3 classes.
validation set:1165 validated image filenames belonging to 3 classes.
test set:2498 validated image filenames belonging to 3 classes.

Model parameters
Total params: 23,688,769
Trainable params: 96,853
Non-trainable params: 23,591,916

Test metrics:
Classification Report:
----------------------
               precision    recall  f1-score   support

   Corrosion       0.96      0.85      0.90       838
      Cracks       0.92      0.91      0.92       782
     Healthy       0.88      0.99      0.94       878

    accuracy                           0.92      2498
   macro avg       0.92      0.92      0.92      2498
weighted avg       0.92      0.92      0.92      2498
