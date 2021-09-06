# Neural_Network_Charity_Analysis
##Overview
This project analyzes which charities were more likely to be more successful at using donations and funds. This analysis uses python's TensorFlow library to create, train and evaluate data gathered from historical loans. 

##Results
After reviewing the data, I established that the target variable is the "IS_SUCCESSFUL" column. then the "EIN" and "NAME" columns were removed because they were determined as irrelevant data that would not the model perform better. The remaining columns became the features for the model.

My first attempt at compiling a neuron network consisted of 8 neurons in the first layer and 6 in the second. I started with these parameters as relu does better with nonlinear data, and two layers allows for a second layer to reweight the inputs from the first layer. In my second attempt, I removed the "SPECIAL_CONSIDERATIONS" column to simplify the model. Additionally, I lowered the threshold for the classification column so that there were more unique values from that column. I also added a third layer with 6 neurons apart of it. In my third attempt, I reverted back the threshold for the classification column. I also changed the activation function for the three layers to tanh. I did this to see if it would perform better than the relu function. In my fourth attempt, I removed the " STATUS" column and reverted back to two layers and the relu activation function. Lastly, I changed the neurons to 12 in the first layer and 8 in the second layer. 

##Summary
After all the attempts, I was unable to create a model that could preform a 75% accuracy rating. This might be from removing too many columns, not using the correct activation funcion or not useing the right amount of layers and neurons. These were the main areas I continued the change with little to no improvement. In the future, I would research more about activation functions to make sure that I am always choosing the right one based on the data.
