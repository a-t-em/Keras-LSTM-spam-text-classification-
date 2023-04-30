**Spam Text Classification**<br>
This is a Python script for a spam text classification model. The model is trained using a dataset of SMS messages and can classify new messages as either "spam" or "ham" (not spam).

**Dependencies**<br>
- Keras
- TensorFlow
- Pandas
- NumPy

**Dataset**<br>
The dataset consists of two files provided by [freeCodeCamp](https://www.freecodecamp.org/learn/machine-learning-with-python/machine-learning-with-python-projects/neural-network-sms-text-classifier):
train-data.tsv: used for training the model
valid-data.tsv: used for validating the model

**Model**<br>
The model is a recurrent neural network (RNN) with two LSTM layers and two dense layers. The input to the model is a sequence of characters and the output is a probability indicating the likelihood of the message being spam. The model is trained on two versions of the input data: one with only alphabetic characters and one with alphanumeric characters.

**Usage**<br>
To use the model, run the script and call the predict_message() function, passing in the message you want to classify as an argument. The function will return a list containing the probability and the label ("spam" or "ham").
