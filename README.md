# British-Sign-Language-BSL-Recognition

This project implements a hand gesture recognition system for **British Sign Language (BSL)** numbers and alphabet using **MediaPipe hand landmarks** and a custom-trained **PyTorch neural network**. The system learns to classify hand poses into corresponding BSL letters and numbers, and can be extended for real-time recognition.

---

## 📂 Dataset

The dataset used is from Kaggle:  
[BSL Numbers & Alphabet Hand Position For MediaPipe](https://www.kaggle.com/datasets/erentatepe/bsl-numbers-and-alphabet-hand-position-for-mediapipe/data)

- Contains MediaPipe-extracted **21 hand landmark coordinates**  
- Includes **alphabet letters (A–Z)** and **numbers (0–9)**  
- CSV format with labeled samples  

---

## ⚙️ Technologies Used

- **Python 3.10+**  
- **PyTorch** – model training & inference  
- **MediaPipe** – hand landmark extraction  
- **NumPy / Pandas** – data preprocessing  
- **Matplotlib / Seaborn** – visualization  

---

## 🚀 Project Workflow

1. **Data Preprocessing**  
   - Load and normalize dataset  
   - Encode labels  

2. **Model Architecture**  
   - Multi-Layer Perceptron (MLP)  
   - ReLU activations, Dropout regularization  
   - Softmax output for classification  

3. **Training & Evaluation**  
   - Loss: CrossEntropyLoss  
   - Optimizer: Adam  
   - Evaluation with accuracy & confusion matrix  

4. **Real-Time Inference (Optional)**  
   - Capture webcam feed  
   - Extract hand landmarks with MediaPipe  
   - Predict BSL letter/number with trained model  

---

## 📊 Results

- Achieved **~94% test accuracy** on the dataset  
- Model successfully distinguishes between BSL numbers and letters  

---

## 📦 Installation

Clone the repository:  
```bash
git clone https://github.com/yourusername/British-Sign-Language-BSL-Recognition.git
cd British-Sign-Language-BSL-Recognition
