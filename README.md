# Attention! LSTMs
A set of notebooks that explores the power of Recurrent Neural Networks (RNNs), with a focus on LSTM, BiLSTM, seq2seq, and Attention.

## English to Italian Machine Translation with BiLSTM and Attention

### Model
Performing machine translation between English and Italian using an __encoder-decoder-based seq2seq model__ combined with __an additive attention mechanism__. The encoder is a Bi-directional LSTM and the decoder is a simple LSTM. The additive attention mechanism is proposed by Bahdanau et al., in their paper [*Neural Machine Translation By Jointly Learning to Align and Translate*](https://arxiv.org/pdf/1409.0473.pdf) published in 2015. [The model](https://drive.google.com/file/d/19GKbKLdNRd_j5RK1Btg-jfTdEvjA41YT/view?usp=sharing) is implemented in Keras.

<img src="./English to Italian Machine Translation with BiLSTM and Attention/attention.png">

### Dataset
The word feature vector data is retrieved from [*nlp.standford.edu.*](https://nlp.stanford.edu/data/glove.6B.zip) and is approximately 350MB in size. The data of English-Italian tab-delimited sentence pairs, which is originally collected for the Tatoeba Project, is retrieved from [manythings.org](http://www.manythings.org/anki/), and is approximately 50MB in size. The training time is within 2 hours (for 35 epochs).

## rnn-chopin-music-generation

### Model
Generating music using a __Recurrent Neural Network (RNN) model with LSTM and dense layers__, implemented in Tensorflow/Keras and trained on 10 pieces of Frédéric Chopin's Waltz/Valse pieces and 9 pieces of Chopin's Nocturne pieces separately.

### Dataset
* 10 Valse/Waltz pieces in MIDI: [kunstderfuge.com](kunstderfuge.com)
* 9 Nocturne pieces in MIDI: [8notes.com](8notes.com)

### Listen to generated sample
[Listen](https://drive.google.com/file/d/15_iUzKmi_8AfiSeuUitjohxkX-sYhoJz/view?usp=sharing) to one of the waltz music generated by the model.
