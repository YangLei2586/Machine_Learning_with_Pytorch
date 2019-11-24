# Machine_Learning_with_Pytorch
Model building and Optimization with Pytorch and Python  
## Pytorch Project 001 Create Linear Regression Model using Pytorch 
### 1 Environment Configuration: Window 10 and Jyputer Notebook 
### 2 Libaries: Torch, torch.nn, torch.autograd, numpy
### 3 Steps
####  Step 1 : Create Dataset 
####  Step 2 : Create Model Class and notice this Model Class is heriated from the nn.Module
####  Step 3 : Specify Loss function and Function Optimizer
####  Step 4 : Create For loop for epoch iteriations
####  Step 5 : Print and Check the model performance by checking the loss decrease over time 

## Pytorch Project 002 Create a Function for Choosing the Best Training Datasize for LSTM Models

#### The batch size and training size will both effect our model prediction preformance. We can manually to choose our traing size but it's better to define a simple but efficient function to let the machine to help us decide the optimal training size efficiently based on the rule of the Stateful LSTMs Model training set size must be divisible without remainder by the batch size. 

#### There are two type LSTM models, which are Stateful LSTM Models and Steteless Models.   

#### Stateless: In stateless LSTMs mode, LSTM updates parameter on batch one, when batch two comes, it will initiate hidden states and cell states with zeros in the batch two. One batch was past then everything is going to be reset and initialized with zeros and then it starts again and again. We use stateless LSTMs when the data are completely unrelated to each other.

#### Stateful: the last output of the hidden state and of the cell states will be the input for the next batch. LSTMs memorizes what it has learned in the previous batch and pass it over to the next batch.  We use stateful LSTMs for time series data such as stock and commodities prices prediction.  

