# Epileptic Seizure Prediction Using Deep Learning

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

- **Machine Learning Application**: The model classifies raw EEG signal data into pre-ictal and inter-ictal periods.
- **Dataset Used**: CHB-MIT EEG dataset with 664 EEG files and 198 seizures.
- **Real-time Prediction**: The model can classify EEG data in real-time, allowing early detection of impending seizures.
- **Pre-emptive Medication**: By detecting pre-ictal periods, the system can trigger alarms to remind the patient to take medication, potentially reducing the impact of seizures or preventing them.

## Visuals

![Block Diagram](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/2.jpg?raw=true)

![Model Architecture](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/3.jpg?raw=true)

![Block Diagram](https://github.com/sam189239/Epileptic-Seizure-Prediction/blob/main/images/5.jpg?raw=true)

## Installation

1. Clone the repository:
   `git clone https://github.com/sam189239/Epileptic-Seizure-Prediction.git`

2. Install dependencies:
   `pip install -r requirements.txt`

## Usage

1. Load the dataset:
   - The CHBMIT EEG dataset must be downloaded and placed in the appropriate directory.

2. Train the model:
   - Use the provided training scripts to train the model using the EEG data.

3. Real-time Inference:
   - The trained model can be used to make real-time predictions by feeding it live EEG data, allowing for early detection of pre-ictal periods.

## License

This project is licensed under the MIT License.
