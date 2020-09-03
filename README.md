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
