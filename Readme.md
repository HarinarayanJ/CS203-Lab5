Group 12

Harinarayan J (23110128) and Vyomika Vasireddy (23110363)

# Files:

"Main.ipynb" has the solution code for the assignment on the given datasets and configuration.

The other files are the same code run on different splits of the same dataset - on the train dataset, with different number of epochs, etc.

# Inferences:

#### Main (25 epochs on given config)

| Metrics | Original | Augmented |
| -------- | -------- | -------- |
| Accuracy | 0.46 | 0.43 |
| Precision | 0.46 | 0.44 |
| Recall | 0.43 | 0.5 |
| F1 Score | 0.44 | 0.47 |

It can be observed that there is no significant change in both the models as the data set size is very low and there isn't much information gain from the augmentations as they are randomly selected from a set of ten augmentations which might not be very helpful. </br>


</br>

#### Main_10Ep (10 epochs on given config)

| Metrics | Original | Augmented |
| -------- | -------- | -------- |
| Accuracy | 0.57 | 0.64 |
| Precision | 0.63 | 0.61 |
| Recall | 0.36 | 0.79 |
| F1 Score | 0.45 | 0.69 |

It can be observed that there is an increase in accuracy and a significant increase in recall with the augmentations. This indicates that the augmentations were helpful and were able to give some information gain. 

</br>

#### Train_Test_Model (10 epochs on entire train set from the original datset)

| Metrics | Original | Augmented |
| -------- | -------- | -------- |
| Accuracy | 0.59 | 0.61 |
| Precision | 0.58 | 0.57 |
| Recall | 0.64 | 0.89 |
| F1 Score | 0.61 | 0.69 |

It can be observed that while there isn't a significant increase in accuracy, it can be observed that there is a significant increase in the recall, indicating that the model has improved in identifying the true positives. Therefore, using more training data shows the usage of augmentations. 
