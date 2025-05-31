# 🗣️ Accent-Agnostic Speech Transcription Model for Enhanced Accessibility

This project addresses the challenge of accent variability in speech recognition, particularly within **e-learning environments**, by developing a **robust, accent-agnostic speech transcription system** using **deep learning techniques**. Leveraging MFCCs for feature extraction and comparing RNN, LSTM, and GRU architectures, the GRU-based model demonstrated superior performance, making a meaningful step toward **inclusive and accessible education** for all.

---

## 🧠 Project Overview

- 🎯 **Objective**: Build a speech recognition model that performs accurately across diverse English accents to improve transcription reliability in digital learning environments.
- 📦 **Dataset**: [Mozilla Common Voice](https://commonvoice.mozilla.org/) – multilingual dataset rich in diverse accents.
- 🔍 **Techniques Used**:
  - Feature Extraction: Mel-Frequency Cepstral Coefficients (MFCCs)
  - Models: RNN, LSTM, GRU (evaluated comparatively)
  - Frameworks: TensorFlow, Keras, NumPy, Matplotlib

---

## 🛠️ Technologies Used

| Category       | Tools/Methods                    |
|----------------|----------------------------------|
| Feature Extraction | MFCCs (LibROSA)              |
| Deep Learning  | RNN, LSTM, GRU (Keras/TensorFlow)|
| Data Handling  | NumPy, Pandas                   |
| Visualization  | Matplotlib, Seaborn             |
| Audio Conversion | FFmpeg                        |

---

## 📈 Performance Summary

| Model | Training Accuracy | Validation Accuracy | Training Loss | Validation Loss |
|-------|-------------------|---------------------|---------------|-----------------|
| RNN   | 75.2%             | 72.8%               | 0.88          | 0.93            |
| LSTM  | 81.4%             | 79.5%               | 0.65          | 0.70            |
| **GRU**   | **83.9%**         | **82.3%**               | **0.59**          | **0.62**            |

> ✅ **GRU outperformed** all other models in accuracy and generalization, proving most suitable for accent-agnostic transcription.

---

## 🔄 Methodology

1. **Data Preprocessing**
   - MP3 → WAV conversion using FFmpeg
   - Resampling to 16kHz
   - Feature extraction using MFCCs
   - Data normalization for convergence

2. **Model Development**
   - Built and compared 3 models: RNN, LSTM, GRU
   - Applied Dropout and TimeDistributed Dense layers
   - Used Categorical Crossentropy loss with Adam optimizer

3. **Evaluation Metrics**
   - Accuracy, Training/Validation Loss
   - Model convergence trends
   - Practical generalization across accents

---

## 💡 Key Findings

- GRU model provided the best trade-off between **computational efficiency** and **performance**.
- LSTM showed solid performance but was more resource-intensive.
- Basic RNN struggled with long-term dependencies and showed signs of overfitting.

---

## 🧩 Applications

- 🎓 **E-learning**: Enhanced subtitle generation and real-time voice recognition for diverse learners
- 🧏 **Accessibility**: Assistive tools for users with hearing impairments or non-native accents
- 💼 **Voice-activated services**: Can generalize well in multilingual call centers or smart assistant platforms

---

## 👥 Team

**Team: Titans Alliance**

- [Bojanapally Santhoshini](https://github.com/Bsanthoshini1811)  
- RamyaSri Muthineni  
- Ruchitha Paccha  

---

## 📚 References

- Mozilla Common Voice Dataset  
- Goodfellow, Bengio & Courville – Deep Learning  
- Graves et al. – Connectionist Temporal Classification  
- Rabiner – Hidden Markov Models in Speech Recognition  
- FFmpeg Documentation

---

## 📬 Contact

For questions or collaborations, feel free to reach out via GitHub or email us directly.
---

