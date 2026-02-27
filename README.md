Audio-based Fault Diagnosis of Air Compressors

This project focuses on detecting and classifying faults in air compressors using audio recordings. By analyzing the sound of an air compressor, the system can identify normal operation and various fault conditions, enabling predictive maintenance and reducing downtime in industrial settings.

Dataset

The project uses the Air Compressor Dataset provided by MathWorks:

AirCompressorDataset.zip

The dataset contains .wav audio files organized into folders representing different conditions such as:

Normal operation

Faulty bearing

Air leaks

Other faults

Each folder represents a label for supervised learning.

Features & Methods

Audio Preprocessing using Librosa
:

Loading .wav files

Extracting features like MFCCs, spectrograms, and chroma features

Assigning labels based on folder names

Dataset Analysis:

Visualizing label distribution in training and test sets

Ensuring balanced data splits

Machine Learning / Deep Learning pipeline (future work):

Training classifiers on audio features

Evaluating accuracy, precision, recall, and F1-score

Predicting compressor status for new audio samples.
Usage

Clone the repository:

git clone <your-repo-url>
cd Audio-based-fault-diagnosis-of-air-compressors

Install dependencies:

pip install librosa pandas matplotlib requests

Download and extract the dataset:

python download_dataset.py

Process audio data and visualize label distributions:

python process_audio.py
