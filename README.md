# Apziva-6
Apziva6

## Problem:

We are a technology company working in the Cyber Security industry. We focus on building systems that help individuals and organizations to have safe and secure digital presence by providing cutting edge technologies to our customers. We create products and services that ensure our customers security using data driven technologies to understand whether audio and video media is authentic or fake.

Our goal in this project is to build algorithms that can synthesize spoken audio by converting a speaker’s voice to another speaker’s voice with the end goal to detect if any spoken audio is pristine or fake.

## Approach

Use Tacotron2 TTS to generate the yes data set (fake) and use the Common Voice dataset as our no data set (not fake). To allow our model to compare the audio files, we must first convert the audio files to spectrograms (visual representations of audio) and then we can use Computer Vision techniques and train binary classification model to classify data.

waveform to spectrogram image here

I used a CNN model and achieved val_accuracy of 100% after 5 epochs. One thing of note is that this model is only trained on female voices for both fake and not fake audio.

graph of model epochs here

