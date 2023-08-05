# kNN_Pruning
Percentile Remove of Data Points in Training Dataset Based on Frequency of Nearest Neighbor Usage


Removal of datapoints within the training dataset for kNN will decrease the time necessary for classification/regression of datapoints within the testing dataset
Datapoints in the training dataset are removed based on their frequency of use by other points within the training data
This will inherently remove outliers from the dataset as outliers are less likely to be used as nearest neighbors but could include other datapoints as well depending on the percentile hyperparameter choosen by the user

Hyperparameters choosen by the user: 
1. The number of nearest neighbors to consider for forming the list of frequency used (nbrs = i.e., 4). This value should be 2 or greater but recommended is no more than 10. The first neighbor is itself and will be dropped by the function.
2. The percentile for dropping the most frequently used (k = i.e., 10). This value can be anywhere between 0 and 100 but 0 will result in no dropping and 100 will result in the dropping of every value in the training dataset. It is recommended to keep this value between 0 and 15.

   
