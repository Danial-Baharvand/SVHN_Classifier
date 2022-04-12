# SVHN_Classifier

This model aims to classify the data from the Street View House Numbers (SVHN) dataset. 3 different methods will be used to achieve this:

1. Train a model from scratch, using no data augmentation, on the abridged SVHN training set.
2. Train a model from scratch, using data augmentation, on the abridged SVHN training set.
3. Fine tune an existing model, trained on another dataset, in this case vgg6-CIFAR10 , on the abridged SVHN training set. CIFAR10 is used due to its similar image size and colour characteristics. However, its classes are named between 0 and 9 whereas the SVHN dataset has its classes between 0 and 10. Therefore the last 3 layers of the model is recreated to enable its use on SVHN.
