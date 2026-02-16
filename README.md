# 🧠 CMPE 258 - Assignment 1D: MNIST Neural Network Classifier

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/258-Assignment_1/blob/main/1D/258_Assignment_1D_Yashaswini.ipynb)

## 📹 Demo Video
[Watch the Demo Video](https://youtu.be/YOUR_VIDEO_ID)

## 👤 Author
**Yashaswini Dinesh**  
Master's Student, Software Engineering  
San José State University

---

## 📋 Overview

This notebook builds and compares neural network models for MNIST digit classification using TensorFlow/Keras.

| Model | Architecture | Test Accuracy |
|-------|-------------|---------------|
| 🔵 Baseline | Flatten → Dense(128) → Dense(64) → Dense(10) | ~97-98% |
| 🟢 CNN | Conv2D → MaxPool → Conv2D → MaxPool → Dense | ~99%+ |

---

## 🚀 Quick Start

### Prerequisites
- Google Colab account
- GPU runtime recommended (faster training)

### Running the Notebook

1. **Open in Colab** - Click the badge above
2. **Select GPU Runtime** - Runtime → Change runtime type → GPU
3. **Run All Cells** - Runtime → Run all

---

## 📁 Output Structure

```
outputs/
├── plots/
│   ├── mnist_samples.png           # Dataset visualization
│   ├── baseline_training_curves.png # Baseline model training
│   ├── cnn_training_curves.png      # CNN model training
│   ├── confusion_matrix.png         # Confusion matrix heatmap
│   └── prediction_grid.png          # Sample predictions
├── metrics/
│   ├── confusion_matrix.txt         # Confusion matrix (text)
│   └── classification_report.txt    # Precision/Recall/F1
└── models/
    └── mnist_cnn.keras              # Saved CNN model
```

---

## 📖 Notebook Sections

### 1. Environment Setup
- Install TensorFlow, scikit-learn, matplotlib
- Set random seeds for reproducibility
- Create output directories

### 2. Load & Explore MNIST
- 60,000 training images, 10,000 test images
- 28×28 grayscale images of digits 0-9
- Normalize to [0, 1] range

### 3. Baseline Model
- **Architecture**: Flatten → Dense(128, ReLU) → Dropout(0.2) → Dense(64, ReLU) → Dropout(0.2) → Dense(10, Softmax)
- **Parameters**: ~118K trainable parameters
- **Training**: 10 epochs, batch size 128

### 4. CNN Model
- **Architecture**:
  - Conv2D(32, 3×3) → BatchNorm → MaxPool(2×2)
  - Conv2D(64, 3×3) → BatchNorm → MaxPool(2×2)
  - Conv2D(64, 3×3) → BatchNorm
  - Flatten → Dense(64, ReLU) → Dropout(0.5) → Dense(10, Softmax)
- **Parameters**: ~93K trainable parameters
- **Training**: 15 epochs with EarlyStopping

### 5. Model Comparison
- Side-by-side accuracy and loss comparison
- CNN typically achieves 1-2% higher accuracy

### 6. CNN Metrics
- **Confusion Matrix**: True vs Predicted labels
- **Classification Report**: Per-class precision, recall, F1-score
- **Prediction Grid**: Visual sample predictions

### 7. Save Model
- Model saved in Keras format (.keras)
- Can be loaded for inference without retraining

---

## 📊 Sample Results

### Training Curves
| Baseline Model | CNN Model |
|----------------|-----------|
| ![Baseline](outputs/plots/baseline_training_curves.png) | ![CNN](outputs/plots/cnn_training_curves.png) |

### Confusion Matrix
![Confusion Matrix](outputs/plots/confusion_matrix.png)

### Sample Predictions
![Predictions](outputs/plots/prediction_grid.png)

---

## 🛠️ Technologies Used

- **TensorFlow 2.x** - Deep learning framework
- **Keras** - High-level neural network API
- **scikit-learn** - Metrics (confusion matrix, classification report)
- **matplotlib** - Visualization

---

## 📝 Key Learnings

1. **CNNs outperform Dense networks** for image classification
2. **Batch Normalization** helps training stability
3. **Dropout** prevents overfitting
4. **EarlyStopping** saves training time
5. **Confusion matrices** reveal per-class performance

---

## 🔗 References

- [MNIST Database](http://yann.lecun.com/exdb/mnist/)
- [TensorFlow Documentation](https://www.tensorflow.org/tutorials/quickstart/beginner)
- [Keras Sequential API](https://keras.io/guides/sequential_model/)
- [CNN for MNIST](https://www.tensorflow.org/tutorials/images/cnn)

---

## ✅ Assignment Requirements Checklist

- [x] Use TensorFlow/Keras (not PyTorch)
- [x] Load MNIST from keras.datasets
- [x] Build baseline model (Flatten + Dense)
- [x] Build improved CNN model
- [x] Compare models (accuracy + loss)
- [x] Training curves saved as PNG
- [x] Confusion matrix (TXT + PNG)
- [x] Classification report (TXT)
- [x] Sample prediction grid (PNG)
- [x] Save CNN model (.keras)
- [x] Clear markdown explanations
- [x] Robust, clean code
- [x] Summary of generated files
- [x] GitHub checklist
- [x] YouTube walkthrough script

---

## 📄 License

This project is for educational purposes as part of CMPE 258 coursework at San José State University.

---

*Last Updated: February 2025*
