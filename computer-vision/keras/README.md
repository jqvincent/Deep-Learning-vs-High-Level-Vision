### Misclassification Rate

The misclassification rate allows to remove biases of our dataset, as described in section 3.3 of our publication.
First, <em>misclassification\_rate\_iterate.py</em> applies many cross-validations on the dataset. 
After each iteration, the predictions on a random validation set are written in a csv file.
Second, <em>misclassification\_rate\_list.py</em> reads the csv files and sums up the number of misclassifications for each image.

### Fine-tuning

First, <em>ft\_presplit\_numpy\_datagen.py</em> to fine-tune on the training set and validate on the validation set.
Second, <em>load\_inf\_numpy\_datagen.py</em> to load the fine-tuned model and apply on the test set.


