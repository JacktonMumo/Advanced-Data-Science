## summary Day 2
* steps to deep learning Analysis
    1. load the data
    2. data cleaning
    3. data preprocessing
    4. create and evaluate the model
    5. make predictions (visualization)
## Activation function
* it is a mathematical equation that determines whether a node should be activated or not
* types of functions
    1. Sigmoid - range(0-1), best for classification
    2. Hyperbolic Tangent(Tanh) - range(-1 to 1), best for regression and classification
    3. ReLU (Rectified Linear Unit) - range(0 to  positive infinity), best for regression
    4. linear - range(no range)

## loss Function
* it calculates the difference between the predicted value and the actual value
* types of functions
    1. Mean Squared Error
    2. Binary Cross-Entropy
    3. Cross-Entropy(Logarithmic)

## Optimizer
* it adjust the weights and bias so as to reduce the loss function
* types of optimizers
    1. Gradient Descent(GD): a fundamental optimizer that updates weights in the opposite direction of the gradient(steepest descent)
    2. Root Mean Squared prop(RMSprop)- adapts the learning rate for each weight based on its recent squared gradient
    3. Adam(Adaptive Moment Estimation): combines RMSprop and momentum, often considered a good default choice due to its effectiveness and ease of use.
## Verbose
* it refers to the amount of info that a model or algorithm outputs during its training or evaluation or execution. this info typically details about the progress of the training process such as loss values, accuracy metrics
* the common levels of verbose are:
    1. 0: No output
    2. 1: Output progress info (eg, one line per epoch)
    3. 2: Output more detailed info(eg progress for each batch within an epoch)