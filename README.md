# Voice Cloning
 
I used Coqui TTS to synthesize speech on a model trained on the TIMIT dataset. There are instructions on how to fine tune a pretrained model in the documentation which can be found here: https://tts.readthedocs.io/en/latest/index.html.
The voice cloning notebook shows the steps to train a model on the TIMIT dataset.

I used the synthesized speech from the Coqui TTS model to create cloned voices and I used real voices from the Mozilla Common Voice Dataset to create a dataset to be used for voice classification. I created a couple neural networks to perform voice classification between real and cloned voices using the dataset, which can be found in the Voice Classification notebook.
The Mozilla Common Voice Dataset can be found here: https://commonvoice.mozilla.org/en/datasets


## Simple Dense Neural Network
<img src='https://i.imgur.com/cybfFGI.jpg'>
<img src='https://i.imgur.com/9ZQdvMl.jpg'>

- Accuracy: 98.9%
- F1-Score: 98.9%

## LSTM Model
<img src='https://i.imgur.com/hEgXmK4.jpg'>
<img src='https://i.imgur.com/Gt5BIZo.jpg'>

- Accuracy: 97.2%
- F1-Score: 97.1%

# Conclusion

I am able to distinguish between real and cloned voices with an extremely high accuracy rate using neural networks. I used a simple feed forward neural network which achieved a 98.9% accuracy rate and an LSTM model which achieved a 97.2% accuracy rate. I would use the simple feed forward neural network with my dataset because it achieved a higher accuracy rate with a shorter training time than the LSTM model.
However, different models could perform better on different datasets, so I would recommend training a couple different models and finding the one that works best for your dataset.









fFlOt7W5debqhiUf