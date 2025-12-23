# 🌿 Plant Disease Classification using Sequential CNN

A deep learning project that classifies **38 plant disease categories** from leaf images using a **custom-built Convolutional Neural Network (CNN)**.  
The project follows an end-to-end machine learning workflow—from dataset exploration to model training, evaluation, and saving for deployment.

---

## 🚀 Project Overview

- **Objective**: Automatically detect and classify plant diseases from leaf images
- **Model Type**: Custom Sequential CNN
- **Classes**: 38 plant disease categories
- **Dataset**: PlantVillage Color Image Dataset
- **Framework**: TensorFlow / Keras

This project demonstrates practical experience with **computer vision, CNN architecture design, data augmentation, and model evaluation**.

---

## 🧠 Key Features

- 📊 Dataset exploration & visualization
- 🖼️ Image preprocessing and normalization
- 🔄 Data augmentation with training/validation split
- 🧱 Custom CNN architecture (no transfer learning)
- ⏹️ Early stopping to prevent overfitting
- 💾 Model checkpointing & saving
- 📈 Performance evaluation on validation data

---

## 🛠️ Tech Stack

- **Python**
- **TensorFlow / Keras**
- **NumPy**
- **PIL (Pillow)**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**

---

## 📁 Project Structure
```
plant-disease-classification/
│
├── dataset/
│ └── plantvillage dataset/
│ └── color/
│
├── model_v2.h5 # Final trained model
├── best_model.h5 # Best model (checkpoint)
├── plant_disease_cnn.ipynb # Training & evaluation notebook
└── README.md
```

---

## 📊 Dataset Details

- **Source**: PlantVillage Dataset
- **Image Type**: RGB leaf images
- **Total Classes**: 38
- **Split**:
  - Training: 80%
  - Validation: 20%

Each class represents a **crop–disease combination**, including healthy leaves.

---

## 🧱 Model Architecture

- **4 Convolutional Blocks**
  - Filters: 32 → 64 → 128 → 128
  - Batch Normalization
  - Max Pooling
- **Global Average Pooling**
- **Fully Connected Layers**
  - Dense (512) + Dropout
  - Dense (256) + Dropout
- **Output Layer**
  - Softmax activation
  - 38 classes

---

## ⚙️ Training Configuration

- **Image Size**: 224 × 224
- **Batch Size**: 16
- **Optimizer**: Adam (Learning Rate = 0.001)
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy
- **Epochs**: Up to 10 (with early stopping)

---

## 📈 Model Evaluation

The model is evaluated on the validation dataset using:

- Validation Loss
- Validation Accuracy


---

## 💾 Saving & Loading the Model

The trained model is saved in `.h5` format and can be reused for inference or deployment.

```python
model.save('model_v2.h5')
```
## 🔮 Future Improvements

- 🚀 Implement **transfer learning** using pre-trained models such as **ResNet**, **EfficientNet**, or **MobileNet**
- 📉 Address **class imbalance** using techniques like class weighting or oversampling
- 🌐 Deploy the model as a **web or mobile application**
- 📷 Enable **real-time plant disease detection** using live camera input
- 📊 Add **confusion matrix** and **per-class performance metrics** for deeper evaluation

---

## 🧑‍💻 Author

**Mridul Kumar**  
📧 Email: **mridulmkumar07@gmail.com**

---

## 📄 License

This project is licensed under the **MIT License**.

---

If you want, I can also:
- ⭐ Add **badges** (TensorFlow, Python, accuracy, etc.)
- 📊 Include **training curves & sample predictions**
- 🧾 Make a **resume-optimized version**
- 🌐 Write a **deployment README** (Flask / FastAPI)

Just say the word 👌

