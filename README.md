# 🎵 Music Genre Classification using Transfer Learning (MobileNetV2)

This project classifies music genres using spectrogram images and a deep learning model built on top of **MobileNetV2**.  
The dataset used is the **GTZAN Music Genre Dataset**, where audio files are converted into spectrogram images for training.

---

## 🧠 Model Architecture
- **Base Model**: MobileNetV2 (pre-trained on ImageNet, frozen at first)  
- **Head**:  
  - Global Average Pooling  
  - Dense layer (128 units, ReLU)  
  - Dropout (0.5)  
  - Dense output layer (10 units, Softmax)  

---

## 🚀 Training
**Key techniques used to improve generalization**:  
- **Optimizer**: Adam (learning rate = 1e-4)  
- **Loss**: Categorical Crossentropy  
- **Metrics**: Accuracy  

