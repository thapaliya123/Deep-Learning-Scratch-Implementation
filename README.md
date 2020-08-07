# cat_dog_predictions
predicts cats and dogs using deep neural  network implemented from scratch allowing to choose different optimization algorithm i.e Adam or Gradient descent as well as different regularization method either dropout or L2 regularization but not both at a time.

# Notebooks
This project has mainly five notebooks i.e ipynb
1. creating_training_dataset.ipynb
- This notebook is capable of creating pickle file of the data stored in directory
- Download cat and dog datasets from kaggle from below link
  https://www.kaggle.com/tongpython/cat-and-dog
- pass training_set path in this notebook and stored in __DATADIR_TR__ variable
- pass test_set path in this notebook and stored  in __DATADIR_TEST__ variable
- Finally, run the notebook and it will generate X_train.pickle, Y_train.pickle, X_test.  pickle, Y_test.pickle
- This data will be used for training in remaining notebook

2. reg_utils.ipynb
- All the helper function for propagating through the deep network are implemented in this notebook
- load_datasets(), initialize_parameters(), forward_propagation(), compute_cost(), backward_propagation(), predict()

3. optimizers.ipynb
- contains helper function for optimizing parameters  i.e using gradient descent and Adam optimizer
- update_parameters(), update_parameters_with_adam()

4. metrics.ipynb
- contains helper function for plotting cost and calculating accuracy
- plot_cost(), calculate_accuracy()

5. minibatch_gradient_descent.ipynb
- This is the main notebook where all the helper function defined above are called and deep neural network is trained, train accuracy and test accuracy are calculated and prediction are made using the learnt parameters.Following are the steps:
- import all the helper function from above ipynb file
- loads training data and testing data from X_train.pickle, Y_train.pickle, X_test.pickle and Y_test.pickle
- creates batches from training set 
- trained the deep neural network
- plot cost
- calculates train and test accuracy
- predicts on new image using learned parameters

# Running project
1. Runnning in colab
- Keep all ipynb file and pickle file in single folder in google drive
- put respective ipynb file id stored in google drive to minibatch_gradient_descent.ipynb file by default id will be stored of mine
- Run minibatch_gradient_descent.ipynb file in colab




