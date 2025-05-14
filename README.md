# MNIST & Fashion-MNIST Classification (FFNN vs CNN)

This project compares two types of neural networks — **Feedforward Neural Network (FFNN)** and **Convolutional Neural Network (CNN)** — on two popular image datasets:
- **MNIST** (handwritten digits)
- **Fashion-MNIST** (Zalando's fashion items)

The goal is to analyze performance differences between basic and deep architectures using clean, standardized datasets.


## Datasets Used

1. **MNIST Dataset**
   - 28x28 grayscale images
   - 10 classes (digits 0–9)

2. **Fashion-MNIST Dataset**
   - 28x28 grayscale images
   - 10 classes (e.g., Shirt, Sneaker, Bag)

Both datasets are included via `tensorflow.keras.datasets`.

---

## Models Compared

### 1. **Feedforward Neural Network (FFNN)**
- Flatten -> Dense(128) -> Output(10)
- Simple structure, no spatial feature extraction

### 2. **Convolutional Neural Network (CNN)**
- Conv2D -> MaxPooling -> Dropout -> Flatten → Dense layers
- Captures spatial features and improves accuracy

---

## 🎯 Results Summary

| Dataset        | Model Type | Accuracy (Test) |
|----------------|------------|-----------------|
| MNIST          | FFNN       | ~96.9%            |
| MNIST          | CNN        | ~98.2%          |
| Fashion-MNIST  | FFNN       | ~87.8%            |
| Fashion-MNIST  | CNN        | ~90.9%            |

> CNN outperforms FFNN on both datasets due to its spatial learning ability.
