### Misclassification Rate

The misclassification rate allows to remove biases of our dataset, as described in section 3.3 of our publication.
1. **misclassification\_rate\_iterate.py** applies many cross-validations on the dataset. After each iteration, the predictions on a random validation set are written in a csv file.
2. **misclassification\_rate\_list.py** reads the csv files and sums up the number of misclassifications for each image.

### Fine-tuning

1. **ft\_presplit\_numpy\_datagen.py** to fine-tune on the training set and validate on the validation set.
2. **load\_inf\_numpy\_datagen.py** to load the fine-tuned model and apply on the test set.


