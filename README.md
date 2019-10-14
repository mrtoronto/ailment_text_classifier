# Ailment Text Classifier

## Goal

Using a dataset derived from 8.5 hours of audio, classify text into common symptoms. 

The dataset had both the audio data and the transcriptions as text so models were created for both data types.

## Kaggle Kernal and Data

Original Kaggle Dataset can be found [here](https://www.kaggle.com/paultimothymooney/medical-speech-transcription-and-intent).

My kernal is [here](https://www.kaggle.com/mtqwerty/classifying-ailments-with-text).

My WAV array can be found [here](https://www.kaggle.com/mtqwerty/x-wav-array) but beware, it didn't work for me.

## Project Notes

The RNN on text was very successful. The model showed high accuracy and quick train times. This is probably a result of the short phrases and clean text.

The CNN on the spectrograms was not succesful. There were a couple factors that played into its failure.
  - Creating the spectrograms was very difficult to do efficiently. 
    - The easiest way I found was running the script locally and uploading either the spectrogram images or the array derived from them separately.
  - Even once I got the data onto kaggle, the network could not classify symptoms from the spectrograms. 
 
 I left the CNN code in the notebook for someone wanting to keep going with it. 
