Neural Network Classification with PyTorch

-This project is about using neural networks to classify points into different categories. It uses PyTorch to build and train the models.

-What This Project Does
*Binary Classification (Circles Dataset)
  Classifies points into two categories (0 or 1).
  Uses a simple neural network to separate the points.
*Multi-Class Classification (Blobs Dataset)
  Classifies points into four categories (0, 1, 2, or 3).
  Uses a slightly bigger neural network to make predictions.
-How the Data Looks
*The circles dataset is created using make_circles() from sklearn.datasets.
*The blobs dataset is created using make_blobs().
*Both datasets have 1000 points, each with two features (X1, X2).

-How the Model Works
*Each model has:
  Input Layer: Takes two numbers (X1, X2).
  Hidden Layers: A few layers that help the model learn patterns.
  Output Layer: Gives the final prediction (either 0/1 for binary or 0-3 for multi-class).
  Activation Function:
  *For binary classification, it uses Sigmoid to get values between 0 and 1.
  *For multi-class classification, it uses Softmax to get probabilities for each class.

-Training the Model
*Loss Function:
  BCEWithLogitsLoss() for binary classification.
  CrossEntropyLoss() for multi-class classification.
*Optimizer: SGD (lr=0.1).
*Epochs: 1000 (the model trains 1000 times).
*Accuracy Calculation: Counts how many correct predictions the model makes.
Results
