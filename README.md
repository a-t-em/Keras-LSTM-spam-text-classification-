Utilizes two Keras LSTM models to classify text as spam or not. 
'al_model' is based on an embedding of only alphabetical characters.
'alnum_model' is based on an embedding of alphanumerical characters plus select symbols. 
Yields the possibility that a given text message is 'spam' or 'ham' by averaging results from the two models. 

