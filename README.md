# Seq2Seq-Model-for-Neural-Machine-Translation

You have been provided a DATASET, which contains pairs of the words (x,y) i.e. akhbaar
अख़बार in which the first word is a Latin word( words we usually type while chatting with friends
in WhatsApp) and the second word is its corresponding word in native script. Your main goal is
to train a seq2seq model which takes as input the romanized string and produces the
corresponding word in native script.
For Example, Jabki yah Jainon se km hai. ⇒ जबकि यह जनै ों सेकम है। 

a) Build a seq2seq model which contains the following layers 
(i) input layer for character embeddings
(ii) one encoder which sequentially encodes the input character sequence (Latin)
(iii) one decoder which takes the last state of the encoder as an input and produces one
character output at a time (native).
Please note that the dimension of input character embeddings, the hidden state of
encoders and decoders, the cell(LSTM), and the number of layers in the encoder and decoder
should be passed as an argument.

b) Now train your model using the standard train, test, and val data provided in the dataset.
Try below mentioned hyperparameters and draw the correlation table along with the plot
(loss/accuracy VS. hyperparameter) for LSTM. 
(i) Input embedding size: 16, 64
(ii) number of encoder layers: 1,3
(iii) number of decoder layers: 1,3
(iv) hidden layer size: 16,64
c) Now add an attention network to your LSTM seq2seq model and train your model along
with the hyperparameter tuning. (you can use single or multiple attention layers) 
(i) Plot the accuracy/loss.
(ii) Report the test accuracy.
(iii) Does the attention-based model perform better than the LSTM? Proof to support your
answer.
