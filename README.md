# Spatial Transform Functions

## transform_to_ind()

### Description
**transform_to_ind** is a function designed to decorrelate spatially dependent data, specifically in the continuous univariate case.

### Arguments 
* formula: An object of class "formula" describing the model to be decorrelated.
* trainData: An object of class data.frame containing the training data with the response variable provided.
* trainLocs: A matrix object containing the coordinates of the training data. The dimensions should be 1x2.
* testData: An object of class data.frame containing the data to be predicted.
* testLocs: A matrix object containing the coordinates of the test data. The dimensions should be 1x2.
* MaternParams: A vector of two parameters: range and nugget. Range represents __ and Nugget represents __. The default is NULL (rng, nug).
* smoothness: The smoothness parameter, representing ____. The default is 1/2.
* M: The number of neighbors to consider when creating a correlation matrix for each individual observation. The default is 30.
* ncores: The number of cores to parallelize the process.

  

**back_transform_to_spatial** is used after applying decorrelated data to your given machine learning model 
