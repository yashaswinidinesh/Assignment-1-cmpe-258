# Assignment 1D: MNIST Neural Network Classifier

**Author:** Yashaswini Dinesh  


---

## Overview

Build and compare neural network models for MNIST digit classification.

| Model | Architecture | Test Accuracy |
|-------|-------------|---------------|
| Baseline | Flatten + Dense | ~97-98% |
| CNN | Conv2D + Dense | ~99%+ |

---

## How to Run

1. Open `258_Assignment_1D_Yashaswini.ipynb` in Google Colab
2. Enable GPU: Runtime → Change runtime type → GPU
3. Run all cells
4. Download outputs zip file

---

## Output Files

```
outputs/
├── plots/
│   ├── mnist_samples.png
│   ├── baseline_training_curves.png
│   ├── cnn_training_curves.png
│   ├── confusion_matrix.png
│   └── prediction_grid.png
├── metrics/
│   ├── confusion_matrix.txt
│   └── classification_report.txt
└── models/
    └── mnist_cnn.keras
```

---

## Model Architectures

### Baseline Model:
```
Input (28x28)
→ Flatten
→ Dense (128, ReLU)
→ Dropout (0.2)
→ Dense (64, ReLU)
→ Dropout (0.2)
→ Dense (10, Softmax)
```

### CNN Model:
```
Input (28x28x1)
→ Conv2D (32) + BatchNorm + MaxPool
→ Conv2D (64) + BatchNorm + MaxPool
→ Conv2D (64) + BatchNorm
→ Flatten
→ Dense (64, ReLU)
→ Dropout (0.5)
→ Dense (10, Softmax)
```

---

## Technologies

- TensorFlow / Keras
- Scikit-learn (metrics)
- Matplotlib (visualization)
- NumPy

---

## References

- MNIST: http://yann.lecun.com/exdb/mnist/
- TensorFlow: https://www.tensorflow.org/
- Keras: https://keras.io/
