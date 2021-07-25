<!-- 
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation. -->
# Neural_Network_Charity_Analysis
## Overview of Analysis
In this analysis we will be looking at funding provided by Alphabet Soup to more than 34,000 organizations. We will be building a neural network for machine learning to help predict whether applicants for funding will be succesful if funded by Alphabet Soup. 

## Results
### Data Prepocessing

    -What variables are considered the targets for the model?
        
        - is_successful
    
    -What variables are considered to be features for this model?

        -application_type
        -use_case
        -ask_amt
        -income_amt
        -classification

    -What variables are neither targets nor features, and should be removed from the input data?

        -ein
        -name
        -affiliation
        -organization

### Compiling, Training, and Evaluating the Model

    -How many neurons, layers, and activation functions did you select for your neural network model, and why?

        -5 hidden layers
        -varying neurons from 90 - 15
        -relu to indentify nonlinear characteristics
        -sigmoid to help predict the probability that funding will be successful

    -Were you able to achieve the target model performance?

        -unfortunately the model was never able to meet the target of 75% accuracy

    -What steps did you take to try and increase model performance?

        -dropped additional columns that are unnecesary to the neural network
        -used different activation functions tanh, selu, linear, hard_sigmoid, gelu, and softmax
        -added additional hidden layers
        - increased the number of neurons
        -increased the number of epochs ran in the model
        - decresed the number of epochs 
        
![network_summary](https://user-images.githubusercontent.com/80363261/126896101-80fe2f6a-6d60-4413-b631-0b8995c630f7.png)
![model_accuracy](https://user-images.githubusercontent.com/80363261/126896106-5df31dc7-6093-40ac-9f23-a677c2c11936.png)

## Summary

While this model does a pretty good job at predictin the success of the funding projects more work can be done to optimize the model. Trying to drop additional columns such as the use_case could yeild a more accurate model. Adding more hidden layers and neurons could also help with provideing a more accurate model. Changing the activation functions and also increasing the number of epochs ran in the model could possibly create a more accurate network.
