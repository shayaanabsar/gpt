# Generative Pre-Trained Transformer (GPT)

GPT models consist of stacked transformer decoder blocks. The model is trained to predict the next word given the preceding words.

Here, I have implemented a character-level GPT model (predicts the next character given the preceding characters). Initially the characters are encoded using embeddings and then positional encodings are added. This data is passed into a series of decoder blocks. Finally, this is passed into a linear layer and the softmax function is applied to produce a probability distribution for the next character is. This distribution can then be sampled from. The process is repeated to produce text.

I have trained the model on a dataset consisting of texts written by Shakespeare. The model achieves a loss of roughly 1.5 on the training set and 1.6 on the test set.