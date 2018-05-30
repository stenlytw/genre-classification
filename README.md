# Music Genre Classification
Comparison of music genre classification with spectrogram input vs. raw audio input using 1D & 2D Convolutional Neural Networks. In this experiment, only the first 20 seconds of each audio is used. Each audio samples is split into 10 parts of 2 seconds audio.

## Prerequisites
```
- Python 2
- Numpy
- Matplotlib
- Scikit-learn
- Scikit-plot
- Keras
- Tensorflow
- Kapre
- Librosa
- ffmpeg
```

## Dataset
[GTZAN](http://marsyasweb.appspot.com/download/data_sets/) music genre data set by George Tzanetakis. The dataset consists of 1000 audio tracks each 30 seconds long. It contains 10 genres, each represented by 100 tracks.

## Results (10 epochs)
|   |Confusion Matrix|ROC curve|Test accuracy|
|---|---|---|---|
|Raw audio input with 1D CNN|![raw-conv1d confusion matrix](https://i.imgur.com/bKHeTPc.png)|![raw-conv1d ROC](https://i.imgur.com/jbk7X0Y.png)|0.31|
|Spectrogram input with 1D CNN|![spectrogram-conv1d confusion matrix](https://i.imgur.com/AdTIG5T.png)|![raw-conv1d ROC](https://i.imgur.com/JYHhHPU.png)|0.7372|
|Spectrogram input with 2D CNN|![spectrogram-conv2d confusion matrix](https://i.imgur.com/a2xPa2T.png)|![raw-conv1d ROC](https://i.imgur.com/kqnIEbA.png)|0.686|

#### References:
- Dieleman, Sander, and Benjamin Schrauwen. "[End-to-end learning for music audio](https://ieeexplore.ieee.org/document/6854950)." Acoustics, Speech and Signal Processing (ICASSP), 2014 IEEE International Conference on. IEEE, 2014.
- https://github.com/tuwien-musicir/DL_MIR_Tutorial
- https://github.com/Hguimaraes/gtzan.keras