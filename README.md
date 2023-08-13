# Transfer_learning
Multiclass image classification using resent50 to classify pipelines into corroded, cracked, healthy pipelines (custom data set)
training set: 4662 validated image filenames belonging to 3 classes.
validation set:1165 validated image filenames belonging to 3 classes.
test set:2498 validated image filenames belonging to 3 classes.

Model architecture
Model: "sequential_11"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 resnet50 (Functional)       (None, 2048)              23587712  
                                                                 
 flatten_11 (Flatten)        (None, 2048)              0         
                                                                 
 batch_normalization_21 (Bat  (None, 2048)             8192      
 chNormalization)                                                
                                                                 
 dense_25 (Dense)            (None, 45)                92205     
                                                                 
 dropout_14 (Dropout)        (None, 45)                0         
                                                                 
 batch_normalization_22 (Bat  (None, 45)               180       
 chNormalization)                                                
                                                                 
 dense_26 (Dense)            (None, 9)                 414       
                                                                 
 dropout_15 (Dropout)        (None, 9)                 0         
                                                                 
 batch_normalization_23 (Bat  (None, 9)                36        
 chNormalization)                                                
                                                                 
 dense_27 (Dense)            (None, 3)                 30        
                                                                 
=================================================================
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
