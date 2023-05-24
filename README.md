# Language-translation
This is an implementation of a Neural Machine Translation (NMT) model using Keras and the Seq2Seq architecture with an LSTM encoder-decoder. The model is trained to translate German sentences to English sentences.

Here is a brief description of the code:

1. The code reads a text file containing German-English sentence pairs and preprocesses the data.
2. The length of the sentences in terms of the number of words is analyzed and visualized using histograms.
3. The text is tokenized using the Keras Tokenizer, creating separate tokenizers for English and German.
4. The sequences are encoded by converting the sentences to sequences of integer values and padding them to a fixed length.
5. The data is split into training and testing sets.
6. The NMT model is defined using the Sequential API in Keras. It consists of an embedding layer, an LSTM layer, a repeat vector layer, another LSTM layer, and a dense (softmax) layer.
7. The model is compiled with an optimizer (RMSprop) and a loss function (sparse categorical cross-entropy).
8. The model is trained on the training data using the fit() function, and the best weights are saved using the ModelCheckpoint callback.
9. The training history is plotted to visualize the loss during training.
10. The trained model is loaded, and predictions are made on the test data.
11. The predicted English sentences are decoded from the integer sequences and compared with the actual English sentences.
12. The actual and predicted sentences are displayed in a DataFrame.

Overall, this code demonstrates the training and evaluation of an NMT model for German-English translation using the Seq2Seq architecture. It uses LSTM layers for sequence processing and tokenization for text preprocessing. The model is trained on sentence pairs and can be used to generate translations for German sentences.
