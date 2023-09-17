# drybeanclasssification

In the given scenario machine learning classification task is performed for the requirements. The requirement
specifies developing an automatic detection system which implies the classification of 7 types of dry bean
seeds. The dataset “Drybeandataset” is provided for processing the classification task. The dataset is based
on research that was conducted on 7 types of unique dry beans considering the features including form,
shape, type, and structure based on the market situation. The developed computer vision system was used
to differentiate the different varieties of dry beans with similar features. In the given dataset, the images of
13,611 grains of 7 distinct types of registered dry beans were captured with high resolution camera. The
images obtained are then subjected to separation as well as feature extractions. Finally, a set of 16 features,
4 shape forms and 12 dimensions were obtained from the captured images. However, during the dataset
analysis, it is found that beans of different varieties may appear similar in terms of their size and shape.
This may challenge the classification task.


For the required automatic detection system, we are provided with a dataset called “DrybeanDataset” .
This multivariate dataset is based on the images of seven distinct types of grains that were captured using
a high-resolution camera (1). The data set consists of integer and real data types and is suited for
classification tasks. The data set has 17 columns with 16 features and a class labelling the dry bean type.
There are 13611 instances whose various features are obtained and noted. The instances are classified into
7 different classes depending on the type of registered dry beans. However, it is relevant to note that the
dataset does not provide a clear description about the external discriminatory features for the dimension
and shape features for the bean varieties.

The primary model chosen for the experimentation of the multiclass classification task of the
dry bean dataset is the Support Vector Machine AND Descion tree Classifier. SVM is a supervised machine learning algorithm whose
objective is to find a hyper plane in an N-dimensional space that distinctly classifies the data points .
The ability of SVMs to create a clear decision boundary between classes makes it well suited for multiclass
classification problems. SVM provides better generalization in comparison to other Machine Learning
Models. SVMs are resistant to overfitting and provide more accurate results in comparison to other
algorithms. The main reason behind the choice of SVM is that the SVMS solve a convex optimization
problem to find the optimal decision boundary.
The decision tree classifier creates a tree like structure in which each internal node represents a decision
based on a feature and each leaf node represents a class label or an outcome. Here I have chosen decision
tree as my second model as they can naturally handle multiclass classification due to its tree structure which
allows the creation of branches and leaf nodes corresponding to each class.


For analyzing the efficiency , the model is experimented with optimized hyper parameters and
the manually chosen hyper parameters. The hyperparameter optimization is not typically considered as a
global optimization issue. Hence, it is necessary to optimize these parameters. The optimization is
performed by the application of randomized search on hyperparameters using RandomizedSearchCV of the
sklearn module . It implements a fit and a score method for the same.

Models can be evaluated using the performance metrics including Accuracy, Precision, recall and F1-score.
Here, I have chosen performance metrics, classification report, Confusion matrix and cross validations as
the modes of evaluation for my SVM model.
