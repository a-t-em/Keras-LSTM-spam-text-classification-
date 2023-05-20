**Spam Text Classification**

This repository contains two Python scripts for spam text classification models:
- spam_text_classification_roberta.ipyn: a Kaggle notebook that demonstrates how to use a pretrained model from Hugging Face to classify spam text messages.
- fcc_sms_text_classification.py: a script that trains a recurrent neural network (RNN) with two LSTM layers and two dense layers to classify spam text messages.

*Pretrained Model*

The pretrained model uses a roberta-base model from Hugging Face that has been further trained on a dataset of SMS messages to differentiate between spam and non-spam texts. The RobertaTokenizer is used to tokenize text messages, and the model is trained on a GPU for faster processing. The freeCodeCamp test suite for the Neural Network SMS Text Classifier project is used as a reference for evaluating the performance of the model.<br>
To use the pretrained model, run the notebook and call the predict_message() function, passing in the message you want to classify as an argument. The function will return the predicted label ("spam" or "ham").<br>
Note that to successfully run the notebook, you will need access to wandb, which can be used to track your experiments and visualize your results.

*LSTM Model*

The LSTM model is trained on a dataset of SMS messages provided by freeCodeCamp. The model is a recurrent neural network with two LSTM layers and two dense layers. The input to the model is a sequence of characters, and the output is a probability indicating the likelihood of the message being spam. The model is trained on two versions of the input data: one with only alphabetic characters and one with alphanumeric characters.<br>
To use the LSTM model, run the script and call the predict_message() function, passing in the message you want to classify as an argument. The function will return a list containing the probability and the label ("spam" or "ham").

*Dependencies*

Both models use two files provided by freeCodeCamp:
- train-data.tsv: used for training the model.
- valid-data.tsv: used for validating the model.<br>
You can find more information about the dataset and the task of spam text classification in the [Neural Network SMS Text Classifier project](https://www.freecodecamp.org/learn/machine-learning-with-python/machine-learning-with-python-projects/neural-network-sms-text-classifier).
