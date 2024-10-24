# Linear Vs. MLP-classification

Exploring supervised learning using gradient descent. It compares linear classifiers with multi-layer perceptron (MLP) and examines binary versus multi-class classification. A key focus is implementing and understanding the backpropagation algorithm in neural networks.

See images show training different models, and their results: <br>

![image](./images/one_v_rest.png)

> One-vs-rest for a Multinomial logistic regression <br>


![image](./images/mlp_binary.png)

> Multi-layer perceptron for binary classification - 93.2% accuracy <br>


![image](./images/multi_class_feed_forward_accuracy_training_best_model.png)

> Multi-class feed forward neural network with high accuracy 


## Results from comparing models

Here are the result from comparing the different types of classifiers on both a binary dataset and a multi-class dataset.

### Binary Classification

```text
Accuracy
Classifier               Training Set        Validation Set      Test Set            
================================================================================
Linear Regression        0.7210              0.7600              0.7200              
Logistic Regression      0.7200              0.7540              0.7240              
Multi-Layer Classifier   0.9360              0.9360              0.9020              

Precision
Classifier               Training Set        Validation Set      Test Set            
================================================================================
Linear Regression        0.6575              0.6857              0.6492              
Logistic Regression      0.6623              0.6866              0.6595              
Multi-Layer Classifier   0.8477              0.8843              0.8304              

Recall
Classifier               Training Set        Validation Set      Test Set            
================================================================================
Linear Regression        0.6494              0.7273              0.6294              
Logistic Regression      0.6296              0.6970              0.6193              
Multi-Layer Classifier   0.9481              0.9646              0.9442              
```

### Multi-Class Classification

```text
Accuracy
Classifier                         Training Set        Validation Set      Test Set            
====================================================================================================
One-vs-Rest Classifier             0.7830              0.8260              0.7680              
Multinomial Logistic Regression    0.6710              0.7380              0.6600              
Multi-Class Neural Network         0.8690              0.8760              0.8460              

Precision
Classifier                         Training Set        Validation Set      Test Set            
====================================================================================================
One-vs-Rest Classifier             0.7830              0.8260              0.7680              
Multinomial Logistic Regression    0.6710              0.7380              0.6600              
Multi-Class Neural Network         0.8690              0.8760              0.8460              

Recall
Classifier                         Training Set        Validation Set      Test Set            
====================================================================================================
One-vs-Rest Classifier             0.7830              0.8260              0.7680              
Multinomial Logistic Regression    0.6710              0.7380              0.6600              
Multi-Class Neural Network         0.8690              0.8760              0.8460              
```