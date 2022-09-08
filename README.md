# NextGrowthLabs
Assessment work for hiring process round 1



> Write about any difficult problem that you solved.

- One of the difficult projects I worked on was detection of cattle's menstrual
cycle using IOT devices data. The fundamental science behind it is that during
the menstrual cycle cow's tend to show hyperactivity when compared to normal
days of the month. 

- The IOT device one like a fitbit device when tied around cow's leg detects 
it's movements throughout the day and updates the database every hour. This 
data is fetched from the database and statistical and machine learning model
was developed to detect true menstrual call and alert the farmer about it.

- Some challenges included were too much noise from IOT device, device failures,
silent menstrual cycles, cattle's sickness, lameness, environment factors
affecting cattle's movements etc.



> Explain back propagation and tell us how you handle a dataset if 4 out of 
30 parameters have null values more than 40 percentage.

- In a neural network the initial weights of the nodes are randomly assigned
during forward propagation. The input features are multiplied by the corresponing
weights and summed up along with bias at each node. This value is then transformed
into an output at the last layer of the network.

- As the network generates a final output, the loss function indicates how well
it predicted the output. The network then performs the backpropagation to 
minimize the loss by adjusting weights and biases. The gradient of the loss
function is calculated with respect to each weight in the network.

- The new weight of a node is calculated by subtracting product of learning rate 
(alpha) and partial derivative of loss function from the old weight. This process
of forward and backward propagation continues to make a network learn untill the 
end of an epoch. It takes many epochs for a network to learn the underlying pattern
to give the most accurate outputs.

- If 40% of data is missing or are null values in any column then we can try one 
of the following 4 tackling methods:
    - drop those columns because here we cannot impute such large volume of cells with 
      mean, median, mode or do any of forward/backward filling. 
    - Replace the null values with a random category name if the column type is categorical.
    - Use regression to predict the missing values if these seems a pattern in missingness.
    - Use KNN or Naive Bayes algorithm as they are immune to missing values.

