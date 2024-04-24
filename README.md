# Image Classification on Fashion MNIST Dataset 

### Problem Statement

In the realm of fashion retail, there's a pressing need to efficiently categorize clothing items into distinct classes for better inventory management and customer experience. The project focuses on leveraging the KNN algorithm to classify images from the Fashion MNIST dataset into 10 predefined classes. My goal is to investigate several experiments aimed at improving model performance. These include finding the optimal training dataset size, determining the best approach for dividing data into training and testing sets, conducting a comparative analysis of distance metrics like Manhattan and Euclidean distance for the KNN algorithm, and evaluating how data transformation through PCA influences model accuracy.


### Data Description

The Fashion MNIST dataset (https://www.kaggle.com/datasets/zalando-research/fashionmnist?resource=download) consists of Zalando’s article images. There are 60000 training and 10000 test 28 x 28 greyscale images, each pixel value ranging from 0 to 255 indicating the lightness or darkness of the pixel. The datasets have 785 columns, the first corresponding to the label (0-9 for 10 classes) and the rest representing the 784 (28 x 28) pixel values. 

### Conclusion

1. The performance of KNN models with Euclidean metric and Manhattan distance metric is the same.
2. The accuracy and f1 score are higher after applying Principal Component Analysis, though the difference is not very significant (<1%).
3. The time required for predicting using the KNN model on the test dataset has reduced significantly from 566.628 seconds to 87.051 seconds (84.64 %). This is because performing dimensionality reduction reduces the number of features (d) and hence, the time required for prediction with the KNN model (O(knd)).
4. The classes with the highest and lowest success rates are 1 (Trouser) and 6 (Shirt) respectively and their success rates are 99.08 % and 67.59 % respectively.

