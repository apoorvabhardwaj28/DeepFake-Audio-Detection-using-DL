# Deepfake Audio Detection using Deep Learning

A deep learning-based framework for detecting **synthetic (deepfake) audio** using hybrid neural network architectures trained on spectral audio features.

This research work was **accepted and presented at the IEEE ICICNCT 2025 Conference**.

---
Research Paper DOI Link: https://ieeexplore.ieee.org/document/11232782

# 📌 Project Overview

Recent advancements in generative AI have enabled the creation of highly realistic synthetic voices. While these technologies are useful for applications such as virtual assistants and speech synthesis, they also introduce risks such as:

- Voice impersonation
- Audio-based identity fraud
- Fake media and misinformation
- Security vulnerabilities in voice authentication systems

This project proposes a **deep learning-based detection framework** capable of distinguishing between **real and AI-generated audio** by analyzing spectral characteristics extracted from speech signals.

The framework evaluates multiple deep learning architectures and identifies the most effective model for deepfake audio detection.

---

# 🎯 Objectives

- Develop a deep learning system for detecting **deepfake audio**
- Compare the performance of **multiple neural network architectures**
- Evaluate models across **different dataset variants**
- Identify architectures that generalize well to unseen audio samples

---

# 🧠 Methodology

The proposed system follows a structured deep learning pipeline.

## 1️⃣ Audio Preprocessing

Raw audio signals are converted into spectral representations that can be used as inputs to deep learning models.

### Extracted Features

**Mel Spectrogram**
- Represents frequency distribution of audio signals over time
- Helps models identify frequency-based artifacts in synthetic audio

**MFCC (Mel Frequency Cepstral Coefficients)**  
- Widely used features in speech processing
- Capture important characteristics of human speech signals

These representations help neural networks learn patterns that differentiate **real speech from synthetic speech**.

---

## 2️⃣ Deep Learning Architectures

Multiple architectures were evaluated for the detection task.

### Convolutional Neural Networks (CNN)
Used for extracting spatial patterns from spectrogram representations.

### Recurrent Neural Networks (RNN)
Capture sequential dependencies within speech signals.

### Long Short-Term Memory Networks (LSTM)
Designed to learn long-term temporal dependencies in sequential data.

### Transformer Models
Evaluated for their ability to model complex dependencies in audio sequences.

### Hybrid CNN–LSTM Model
The final model combines:

- CNN layers for **spectral feature extraction**
- LSTM layers for **temporal sequence modeling**

This hybrid architecture achieved the **best performance**.

---

# 📊 Dataset

The dataset used in this project was obtained from **Kaggle**.

Dataset: **Fake-or-Real Audio Dataset**

It contains both:

- Real human speech recordings
- AI-generated synthetic speech samples

To improve evaluation robustness, the study explored multiple dataset variations including:

- Original dataset
- Normalized audio samples
- Short audio segments
- Re-recorded audio samples

These variations simulate real-world audio conditions.

---

# ⚙️ Training Environment

Model training and experimentation were conducted using **Kaggle Notebooks** with GPU acceleration.

**Hardware**

- NVIDIA GPU (Kaggle GPU environment)

**Platform**

- Kaggle Notebook Environment

GPU acceleration significantly reduced training time for deep learning models.

---

# 📈 Results

Extensive experiments were conducted to evaluate model performance.

Key observations:

- Hybrid architectures outperform individual deep learning models
- Spectral features such as MFCC and Mel Spectrograms are highly effective
- The CNN–LSTM hybrid model achieved the best results

### Best Model Performance

**Test Accuracy:** 99.98%

This demonstrates the effectiveness of deep learning models in detecting subtle artifacts present in synthetic audio.

---

# 🛠 Tech Stack

**Programming Language**

- Python

**Deep Learning Frameworks**

- TensorFlow
- PyTorch

**Audio Processing**

- Librosa
- OpenCV

**Data Processing**

- NumPy
- Pandas

**Visualization**

- Matplotlib
- Seaborn
---

# 📄 Research Publication

**Title:**  
Deepfake Audio Detection: A Multi-Model, Multi-Dataset Performance Study using Deep Learning Architectures

**Conference:**  
IEEE ICICNCT 2025  
International Conference on Intelligent Communication Networks and Computational Techniques

---

# 👨‍💻 Author

**Apoorva Bhardwaj**  
Department of Electronics and Communication Engineering  
Sharda University, India

---

# 📜 License

This repository is intended for **research and educational purposes**.
