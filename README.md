# Epileptic Seizure Prediction - ConvLSTM
** Spatio-temporal modeling**

## Objective

The goal of this project is to set up a deep learning prediction model to classify between **pre-ictal** and **inter-ictal** periods using EEG (Electroencephalography) data from patients with epilepsy. The model aims to provide early alarms ahead of an epileptic seizure, allowing patients to take pre-emptive medication, thereby reducing the effects and potential damage caused by seizures or preventing them altogether.

## Data Used

The model is trained using the **CHBMIT Scalp EEG Database**, which contains recordings of EEG signals from 22 subjects (5 males, ages 3–22; and 17 females, ages 1.5–19). The data consists of 664 **edf files**, each containing exactly one hour of digitized EEG signals. These recordings include 129 files with one or more seizures, totaling 198 seizures in the dataset. The EEG signals are sampled at 256 samples per second with 16-bit resolution and are recorded using the **International 10-20 System** for electrode positioning.

- Dataset: [CHBMIT EEG Database](https://physionet.org/content/chbmit/1.0.0/)

## Model Architecture

The model uses deep learning techniques to classify EEG signals into **pre-ictal** and **inter-ictal** periods. It leverages:

- **Convolutional Neural Networks (CNN)** to capture spatial relationships in the EEG signals.
- **Bi-directional LSTM (Long Short-Term Memory)** layers to capture temporal relationships and predict the onset of seizures.

The model can make real-time predictions when fed with live EEG data, allowing for early detection of pre-ictal periods and issuing an alarm for potential seizures.

## Outcomes

- Machine Learning has been employed to classify raw EEG signal data into Pre-ictal and Inter-ictal periods.
- Dataset was manually cleaned and processed (large-scale data processing)
- Classification is carried out on 5-minute intervals of 23-channel EEG signal collected using Brain-Computer Interface.
- The model uses Convolutional layers to find spatial relationships and Bidirectional LSTM layers to find temporal relationships, detecting pre-ictal and inter-ictal periods.
- When this model is fed real-time data, classification can be done in real-time to identify potential pre-ictal periods, allowing pre-emptive indication of an impending Epileptic seizure.
- This alarm would allow for medication to be taken ahead of an Epileptic Seizure to reduce the effects of the seizure or even avoid it entirely.

## Workflows

![Block Diagram](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/2.jpg?raw=true)

![Model Architecture](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/3.jpg?raw=true)

![Block Diagram](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/5.jpg?raw=true)

## License

This project is licensed under the MIT License.
