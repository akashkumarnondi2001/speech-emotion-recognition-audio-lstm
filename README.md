# Speech Emotion Recognition (SER) from Audio Data Using LSTM Model

This repository contains the official source code and implementation for my BSc in Computer Science and Engineering (CSE) thesis. 

The project focuses on **Speech Emotion Recognition (SER)**, utilizing a **Long Short-Term Memory (LSTM)** neural network architecture to process and classify emotional states from raw audio signals.

---

## 📌 Project Abstract
The capacity to comprehend and interact with others through language is a uniquely valuable human ability. Because emotions are crucial to communication, humans are highly trained to recognize and interpret them. However, due to the subjective nature of human mood, emotion recognition remains highly challenging for computers. 

While existing approaches utilize images, text, and multimodal inputs, this work specifically targets **audio datasets** to establish accurate human emotion classification. We implement an LSTM network trained and evaluated on two benchmark datasets: 
1. **RAVDESS** (Ryerson Audio-Visual Database of Emotional Speech and Song)
2. **TESS** (Toronto Emotional Speech Set)

---

## 📊 Performance & Results

Our trained LSTM model achieved highly robust accuracy rates across both distinct and combined datasets:

| Dataset Evaluation | Accuracy Rate |
| :--- | :--- |
| **TESS Dataset** | **98.05%** |
| **RAVDESS Dataset** | **91.25%** |
| **Combined Datasets** | **87.66%** |

These results highlight the effectiveness of the LSTM model in processing sequential audio features and its generalized capability to manage varied datasets.

---

## 🛠️ System Architecture & Features
* **Feature Extraction:** MFCCs (Mel-Frequency Cepstral Coefficients), Chroma, and Mel-scaled spectrograms extracted using `librosa`.
* **Model Pipeline:** Sequential LSTM layers integrated with Dropout and Batch Normalization layers to mitigate overfitting.
* **Classification:** Multi-class classification mapping to primary emotional states (e.g., Happy, Sad, Angry, Fearful, Neutral, Disgust, Surprise).

---

## 🚀 Getting Started

### Prerequisites
Ensure you have Python 3.8+ installed. You can install the required packages using:
```bash
pip install -r requirements.txt
```

### Dataset Structure
Download the datasets from their official sources and organize them as follows:
```text
├── datasets/
│   ├── RAVDESS/
│   └── TESS/
```

### Running the Project
1. **Feature Extraction:** Run `python extract_features.py` to process the audio files.
2. **Training:** Run `python train.py` to train the LSTM network.
3. **Evaluation:** Run `python evaluate.py` to test the model and view confusion matrices.

---

## 🎓 Thesis Context
* **Degree:** Bachelor of Science in Computer Science and Engineering (BSc in CSE)
* **Author:** Author : Md. Mahbub-Or-Rashid, Akash Kumar Nondi, Abdullah Al Sadnun, Md. Anwar Hussen Wadud, T M Amir Ul Haque Bhuiyan, Md. Saddam Hossain
* **Institution:** Bangladesh University of Business and Technology
