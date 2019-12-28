# Fashion_class_classifier

Using **Convolutional Neural Network** to accurately classify clothing and other fashion items from their images.

The Neural Network is trained on a dataset consisting of 60,000 Training and 10,000 Testing dataset in the form of Black and White image pixel points of dimensions [28 x 28]. After training and optimizing the model using variety of techniques, the final Neural model was able to reach an accuracy of **94.42%** and a test accuracy of **91.8%**. Click [here](https://github.com/vaishak47/fashion_class_classifier/blob/master/fashion_classifier.ipynb) to visualise the classification.

### Tools Used
* Jupiter Notebook - for coding and visualizing the data

### Packages used
* Pandas - for Manipulation of data frames
* Numpy - for Statistical analysis
* Matplot - for Data visualization
* Seaburn - for Statistical Data visualization
* SKLearn - for splitting the testing-training dataset
* Keras - Neural network library for deploying the Neural Network

### Source of Training data-set
* **[FashionMNIST dataset](https://www.kaggle.com/zalando-research/fashionmnist/data)** containing 60,000 training and 10,000 testing Image data in Black and White format.
* Advanced [dataset](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) containing images with texture, patterns and color data for further training.

### Methodology for Training the Neural Network
* Convolution of the Raw Image data using **Kernals/Feature Detectors** for feature extraction, thereby prioritizing the imporatant highlights of the image.
* Deploying **Rectified Linear Units (RELU) Activation Function** to add non-linearity in the feature map.
* **Pooling/Down-sampling** to reduce the feature map dimensionality. Here **Maxpooling** is used to improve the computational efficiency while preserving the features.
* Finaly **Flattening** out the down-sampled data into long single dimensional array of values.


### Improving the accuracy of the model by 
* Adding more feature detectors/kernals.
* Using Dropout thereby decreasing the co-dependency of the neuron, hence introducing more generalization.

### Accuracy Obtained
After deploying the above mentioned optimization techniques, the following accuracy rates where obtained.
* 32 kernal without dropout:
    - Accuracy : 0.9585
    - Test Accuracy: 0.912
* 64 kernal without dropout
    - Accuracy : 0.9641
    - Test Accuracy : 0.915
* 64 kernal with dropout
    - Accuracy : 0.9442
    - Test Accuracy : 0.918

