# image-caption-generator

A caption summarising the image is generated when inputted into the model. The model is made up of an encoder and a decoder. 

The encoder is a ResNet50 pre-trained model with a fine-tuned linear layer for extracting the image features. 

The decoder contains an LSTM-based seq2seq architecture with Luong Attention Mechanism to identify the caption. 

The model uses PyTorch to train and evaluate, with average training loss of as low as 2.3370 with a remarkable average BLEU score of 0.4665, and validation loss of around 3.6 with average BLEU score of 0.334. The loss used is Cross Entropy Loss. The model has been trained on the publically available Flickr32K Dataset and can be trained further on larger datasets like MSCOCO for better results and higher generalization. 
