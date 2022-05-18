Objective:

To set up a deep learning prediction model by making use of existing EEG (Electro-encephalography) data of Epileptic Seizures to classify between pre-ictal and inter ictal periods, so as to set up alarms ahead of Epileptic Seizures which would allow the patient to take pre-emptive medication to reduce to effects and damages of the seizure or avoid the seizure entirely. 

Data used: 

The CHBMIT scalp EEG database was used for the training of the model. Recordings, grouped into 23 cases, were collected from 22 subjects (5 males, ages 3–22; and 17 females, ages 1.5–19). The raw EEG signals were sampled at 256 samples per second with 16-bit resolution. Most files contain 23 EEG signals.  The International 10-20 system of EEG electrode positions and nomenclature was used for these recordings. There are 664 edf files included in this collection, which contain exactly one hour of digitized EEG signals, and 129 of those files contain one or more seizures. In all, these records include 198 seizures.


![Block Diagram](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/2.jpg?raw=true)

![Model Architeture](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/3.jpg?raw=true)

![Block Diagram](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/5.jpg?raw=true)

Outcomes:

- Machine Learning has been employed to classify raw EEG signal data into Pre-ictaland Inter-ictal periods.
- Classifier model is trained using CHB-MIT EEG Dataset.
- Classification is carried out on 5-minute intervals of 23-channel EEG signalcollected using Brain-Computer Interface.
- The model makes use of Convolutional layers to find spatial relationships and Bi-directional LSTM layers to find temporal relationships, so as to classify pre-ictal andinter-ictal periods.
- When this model is fed real-time data, classification can be done in real-time so asto identify potential pre-ictal periods, allowing pre-emptive indication of animpending Epileptic seizure.
- This alarm would allow for medication to be taken ahead of an Epileptic Seizure toreduce the effects of the seizure or even avoid it completely. 