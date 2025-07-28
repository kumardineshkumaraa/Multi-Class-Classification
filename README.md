
# Animal Classification using CNN

This project implements a **Convolutional Neural Network (CNN)** to classify images from the **Animals10 dataset** into 10 categories:
`cane`, `cavallo`, `elefante`, `farfalla`, `gallina`, `gatto`, `mucca`, `pecora`, `ragno`, `scoiattolo`.

---

## 📌 Dataset Details
- **Dataset:** Animals10
- **Total Images:** 26,179
- **Classes:** 10 animal categories.
- **Train Set:** 20,944 images
- **Validation Set:** 5,235 images
- Images were resized to 128x128 and normalized before training.

---

## 🧠 Model Architecture
The CNN consists of:
- **3 Convolutional layers** (Conv2D with ReLU activation)
- **3 MaxPooling layers**
- **Flatten layer**
- **Dense layer with 128 units (ReLU)**
- **Softmax output layer** (10 classes)

**Optimizer:** Adam (learning rate = 0.001)  
**Loss function:** Sparse Categorical Crossentropy  
**Epochs:** 10  
**Batch size:** 32  

---

## 📊 Training Results
- **Final Validation Accuracy:** ~85%
- Model converged well after 10 epochs.

---

## ⚠ Challenges and Solutions
- **Overfitting risk** due to dataset complexity → mitigated by reducing model complexity and tuning epochs.
- **Class imbalance** observed → evaluated results carefully and ensured balanced metrics.

---

## Conclusion:
The CNN model achieved a validation accuracy of around 85%, demonstrating strong performance in classifying 10 animal categories. Despite using a relatively simple architecture without data augmentation, the model generalized well. Future improvements, such as transfer learning or hyperparameter tuning, could further enhance accuracy.
