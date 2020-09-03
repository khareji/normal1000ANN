# ANN(Artifical Neural Network)
An ANN is based on a collection of connected units or nodes called artificial neurons, which loosely model the neurons in a biological brain. Each connection,
like the synapses in a biological brain, can transmit a signal to other neurons.
An artificial neuron that receives a signal then processes it and can signal neurons connected to it. 
The "signal" at a connection is a real number, and the output of each neuron is computed by some non-linear function of the sum of its inputs. 
# Aim
To perform ANN in data set to find the output which is in classifed form
# Data
Data ia about a person activity like RowNumber,	CustomerId	,Surname	,CreditScore,	Geography	,Gender,	Age,	Tenure,	Balance,	NumOfProducts,	
HasCrCard,	IsActiveMember	,EstimatedSalary	,Exited(labeled 0 or 1 ).downloaded from kaggle which is about 1000 rows.
# Information
all the features are in number , except geography and gender which is further converted into number using dummies variable
# Procedure
In ANN we have see few thing in starting like weights which are our features values, and activation fucntion which is our relu and sigmoid in our last layer because our labeled data is 0 and 1.
# Modle
sequential model is used This is the simplest model is defined in the Sequential class which is a linear stack of Layers. You can create a Sequential model and define all of the layers in the constructor, for example: from keras.models import Sequential model = Sequential(...)
# Optimzer 
there are different diffferent types of optimizer like gradient descent , adam,adagard , rsmpoop,etc but here is use adam
the use of optimizers in NN is to find the global or local minima which will make predicted value as actual value .
adaptive learning rate optimization algorithm that's been designed specifically for training deep neural networks. ... The algorithms leverages the power of adaptive learning rates methods to find individual learning rates for each parameter.
# loss function
it is use to find the difference between the actual - predicted value ,loss function, that can be used to estimate the loss of the model so that the weights can be updated to reduce the loss on the next evaluation.
Loss functions and optimizations. Machines learn by means of a loss function. It's a method of evaluating how well specific algorithm models the given data.
 
      Regression Loss Functions
         Mean Squared Error Loss
          Mean Squared Logarithmic Error Loss
          Mean Absolute Error Loss
     `Binary Classification Loss Functions
        Binary Cross-Entropy
        Hinge Loss
        Squared Hinge Loss
    `Multi-Class Classification Loss Functions
         Multi-Class Cross-Entropy Loss
         Sparse Multiclass Cross-Entropy Loss
          Kullback Leibler Divergence Loss
    
# sample
A sample is a single row of data.
It contains inputs that are fed into the algorithm and an output that is used to compare to the prediction and calculate an error.
# Batch->10
The batch size is a hyperparameter that defines the number of samples to work through before updating the internal model parameters.
# Epoch ->100
The number of epochs is a hyperparameter that defines the number times that the learning algorithm will work through the entire training dataset.

One epoch means that each sample in the training dataset has had an opportunity to update the internal model parameters. An epoch is comprised of one or more batches. For example, as above, an epoch that has one batch is called the batch gradient descent learning algorithm.

You can think of a for-loop over the number of epochs where each loop proceeds over the training dataset. Within this for-loop is another nested for-loop that iterates over each batch of samples, where one batch has the specified “batch size” number of samples.

The number of epochs is traditionally large, often hundreds or thousands, allowing the learning algorithm to run until the error from the model has been sufficiently minimized. You may see examples of the number of epochs in the literature and in tutorials set to 10, 100, 500, 1000, and larger.
