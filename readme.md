## TransformerTTS

### Overview

This repository is a PyTorch implementation of a neural network-based speech synthesis model, Transformer-TTS, which uses the Transformer Network. It is based on the code by [ChoiHkk's Transformer-TTS](https://github.com/choiHkk/Transformer-TTS/tree/main) and has been trained on the LJSpeech dataset. You can run the [notebook](https://github.com/Orca0917/TransformerTTS/blob/main/TransformerTTS.ipynb) in a Google Colab environment.

<br>

### Model architecture

![Transformer architecture](./assets/transformer-tts-architecture.png)

<br>

### Dataset

The dataset used is the English speech dataset LJSpeech. In the Jupyter notebook, the dataset is utilized without a separate download by using the `torchaudio` package. The data preprocessing was implemented by referring to the tacotron audio preprocessing by [Kyubong Park](https://github.com/Kyubyong).

* https://keithito.com/LJ-Speech-Dataset/
* torchaudio.dataset

<br>

### Result 

The training was conducted with a batch size of 16 on a total of 13,100 voice datasets for 10 epochs. The result is expressed as a gif showing the predicted mel spectrogram and the ground truth mel spectrogram every 100 steps.

![training result](./assets/transformer-tts-result.gif)

<br>
