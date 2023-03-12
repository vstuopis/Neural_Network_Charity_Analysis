# Neural_Network_Charity_Analysis

## Overview

By using machine learning and neural networks, we worked to help Beks create a binary classifier to predict if an applicant will successfully be funded by Alphabet Soup. We worked with a vast dataset of over 34,000 organizations which we processed the data we were provided. We proceeded to compile, train and evaluate the model using TensorFlow. As the results we got were under the 75% threshhold we were looking for, we tried 3 different ways to optimize our model further to get us over the 75% mark.

## Results

### Data Preprocessing
* Model Target
  * IS_SUCCESSFUL
* Model features
  * APPLICATION_TYPE
  * CLASSIFICATION
* Variables neither targets or features which should be removed from input data include
  * EIN
  * NAME
  
![Removed Columns](https://github.com/vstuopis/Neural_Network_Charity_Analysis/blob/main/Dropping%20EIN%20and%20Name.png)

### Compiling, Training, Evaluating the Model
* Neurons, layers, and activation functions selected for your neural network model and why
  * Neurons
    * Layer 1 = 80
    * Layer 2 = 30
  * 2 Layers 
  * Relu Function used other than output layer where sigmoid used
* Able to achieve target model performance
  * No
* Attempts made to increase model performance
  * Increase number of hidden layers
 ![Increase number of hidden layers](https://github.com/vstuopis/Neural_Network_Charity_Analysis/blob/main/Increased%20Hidden%20Layers.png)
  * Change activation functions
 ![Change activation functions](https://github.com/vstuopis/Neural_Network_Charity_Analysis/blob/main/Change%20Activation%20Functions.png)
  * Increase number of nodes in hidden layers
 ![Increase number of nodes in hidden layers](https://github.com/vstuopis/Neural_Network_Charity_Analysis/blob/main/Increased%20Nodes%20in%20Hidden%20Layers.png)
 
## Summary

Overall the results of the deep learning model were unable to achieve the target model performance we were looking for at 75%. The model came close and maybe a few other different optimizations could have gotten us to the target, but for this classification problem a deep learning model may not be the best one to use. I would recommend using the Principal Component Analysis or PCA, model. The reason I would use this model is because I'd want to focus only on the columns in the data set driving most of the model variance and keep the rest of the noise out of the model.
