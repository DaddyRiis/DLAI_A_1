# DLAI_A_1

We create a RNN for TSLA stock data daily going back 5 years. 

We create this RNN to forecast future TSLA pricing based previous prices.

To train the RNN we split the data into a train-test split.

We added a couple of hyperparameters in order to finetune the models capabilities: 
 - Epochs
      - Number of iterations of a sample going through stochastic gradiant descent
 - Learning rate
      - The size of the steps used in the stochastic gradiant descent. Too large steps can results in a too quick convergence, whereas a too small stepsize could results in taking too long to converge. Both could create a suboptimal solution. 
 - Hidden layers
      - Nodes that have the ability to remember the results of previous calculations. Using those stored “memories,” the neural network can then predict the current input based on past results. The deeper and more complicated the problem the RNN has to solve, more layers can help optimize and improve the model, but adding to many can overcomplicate and reduce performance.

We ended up choosing 2 hidden layer, 50 epochs and a learning rate 0,001 be iteratively evaluating the model by plotting the models predictions against the actual prices. Our model with the above setttings, generally underestimates the prices, where a single instance it overestimates the prices. 

