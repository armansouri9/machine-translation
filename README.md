# Text Translation with LSTM

This repository contains code for training a text translation model using LSTM (Long Short-Term Memory) networks. The model is trained to translate input texts from one language to corresponding output texts in another language.

## Dataset

The dataset used for training consists of input texts and their corresponding output texts. Here are a few examples from the dataset:

- Input Text: "How are you?" | Output Text: "I'm fine, thank you."
- Input Text: "What's your name?" | Output Text: "My name is John."
- Input Text: "What do you do?" | Output Text: "I'm an engineer."
- Input Text: "Ali?" | Output Text: "Reza"

## Model Architecture

The text translation model is implemented using PyTorch. It consists of an embedding layer, an LSTM encoder, an LSTM decoder, and a fully connected layer. The model takes an input sequence, encodes it using the encoder LSTM, decodes it using the decoder LSTM, and generates the output sequence. The output sequence is passed through a softmax function to obtain the predicted output probabilities.

## Training

The model is trained using the provided dataset. The training process involves iterating over the dataset for a specified number of epochs. For each input-output pair in the dataset, the model calculates the loss between the predicted output and the actual output using the negative log-likelihood loss (NLLLoss). The optimizer (Adam) is then used to update the model's parameters based on the calculated loss.

During training, the loss is printed for every 10th epoch to monitor the model's progress.

## Inference

After training, the model can be used for text translation. A sample input text, "Ali?", is provided, and the model predicts the corresponding output text. The model's prediction is obtained by passing the input sequence through the trained model, selecting the top-k predictions, and converting them back into text format.

For the given input text "Ali?", the model predicts the output text "Reza".

Please note that this is a simplified example, and further improvements can be made to enhance the model's performance.

Feel free to explore the code and adapt it to your own text translation tasks!
