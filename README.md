# Machine Translation (EN-FA)

This repository contains code for machine translation from English to Farsi (Persian). The code is implemented in a Jupyter Notebook file named "Machine Translation(EN-FA).ipynb". The notebook provides an example of training a translation model using a sequence-to-sequence architecture with an LSTM encoder and decoder.

## Repository Structure

- `Machine Translation(EN-FA).ipynb`: Jupyter Notebook file containing the code for training and testing the translation model.
- `LICENSE`: License file for the project.

## Dataset

The dataset used for training the translation model consists of English input texts and corresponding Farsi output texts. The input and output texts are provided in the code as lists named `input_texts` and `output_texts`, respectively.

## Dependencies

The following Python packages are required to run the code:

- transformers
- torch

Install the required packages using the following command:

```
pip install transformers torch
```

## Training the Model

To train the translation model, run the cells in the Jupyter Notebook file "Machine Translation(EN-FA).ipynb". The notebook includes code for defining the model architecture, creating the translation dataset, training the model using the dataset, and evaluating the model's performance.

## Testing the Model

After training the model, you can test its performance on new input texts. The notebook includes an example of testing the model on the input text "چکار می‌کنی؟" (What do you do?). The predicted output text will be displayed.
## License

This project is licensed under a Free License.
