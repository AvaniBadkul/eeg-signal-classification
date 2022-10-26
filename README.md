# EEG Signal Classification

## Introduction

- EEG stands for electroencephalogram, and it measures the electrical activity in your brain from the synaptic excitations of your neurons’ dendrites.
- The human brain has unique brain wave frequencies. There are five types of brain waves - Gamma, Beta (low, midrange, and high beta as its sub-sections), Alpha, Theta, and Delta waves ordered by the depth of brain waves [[1]](http://dx.doi.org/10.1109/ICDAMT.2018.8376536).


## Data

- The data used for performing classification of EEG signal was taken from [Jordan Bird et al.](https://www.researchgate.net/publication/329403546_Mental_Emotional_Sentiment_Classification_with_an_EEG-based_Brain-machine_Interface)
- The dataset has been processed by Jordan Bird et al.
- The data was collected from two people (one male and one female) for 3 minutes/state - 'positive', 'neutral', 'negative'.

## Code
- The files for each of the models are located in the *Models* folder.
- The code file are Python Notebooks.
- Each file contains a detailed analysis of the model, this includes the ***confusion matrix, precision, recall, f1-score, and support***.
- Libraries Used: numpy, pandas, matplotlib, seaborn, sklearn, tensorflow, and keras.

## Results

- The Table below shows the various models created.
- As shown the best model is *Model 5* in terms of Accuracy and Validation Accuracy.

| Model  | Epochs | Learning Rate | Optimizer |           Loss Function          | Accuracy | Val Accuracy |
|:------:|:------:|:-------------:|:---------:|:--------------------------------:|:--------:|:------------:|
|    0   |   75   |      0.01     |    SGD    | Sparse Categorical Cross Entropy |  96.114  |    97.067    |
|    1   |   75   |     0.001     |    SGD    | Sparse Categorical Cross Entropy |  91.129  |    92.669    |
|    2   |   75   |      0.01     | Adamdelta | Sparse Categorical Cross Entropy |  95.381  |    96.774    |
|    3   |   75   |      0.01     |  Adagrad  | Sparse Categorical Cross Entropy |  95.748  |    97.067    |
|    4   |   75   |      0.01     |   Adamax  | Sparse Categorical Cross Entropy |  95.894  |    96.774    |
|    5   |   75   |     0.001     |   Adamax  | Sparse Categorical Cross Entropy |  99.120  |    98.827    |
|    6   |   75   |     0.001     |    Adam   | Sparse Categorical Cross Entropy |  95.968  |    97.067    |
|    7   |   75   |      0.01     |    Adam   | Sparse Categorical Cross Entropy |  34.091  |    34.311    |
|    8   |   75   |     0.001     |  Adagrad  | Sparse Categorical Cross Entropy |  93.768  |    94.721    |
|    9   |   75   |     0.001     | Adamdelta | Sparse Categorical Cross Entropy |  91.600  |    93.260    |
|   10   |   75   |      0.01     |    SGD    |     Categorical Cross Entropy    |  93.255  |    93.255    |
|   11   |   75   |     0.001     |    SGD    |     Categorical Cross Entropy    |  97.141  |    97.067    |
|   12   |   75   |      0.01     | Adamdelta |     Categorical Cross Entropy    |  95.308  |    95.894    |
|   13   |   75   |      0.01     |  Adagrad  |     Categorical Cross Entropy    |  96.408  |    97.947    |
|   14   |   75   |      0.01     |   Adamax  |     Categorical Cross Entropy    |  94.721  |    94.721    |
|   15   |   75   |     0.001     |   Adamax  |     Categorical Cross Entropy    |  99.047  |    98.240    |
|   16   |   75   |     0.001     |    Adam   |     Categorical Cross Entropy    |  96.701  |    97.067    |
|   17   |   75   |      0.01     |    Adam   |     Categorical Cross Entropy    |  89.956  |    92.669    |
|   18   |   75   |     0.001     |  Adagrad  |     Categorical Cross Entropy    |  93.182  |    94.135    |


### Accuracy of Various Models

![Accuracy of Various Models](https://user-images.githubusercontent.com/79955028/127029438-a536182d-4611-4712-a362-1e45178e16bd.png)

### Validation Accuracy of Various Models

![Validation Accuracy of Various Models](https://user-images.githubusercontent.com/79955028/127029675-442b613f-2ded-41b8-b730-93e1a8952ccd.png)

## Future Work
To implement different and new algorithms.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://github.com/AvaniBadkul/EEG-Signal-classification/blob/master/LICENSE)
