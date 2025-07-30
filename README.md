# 🪸 Corals Image Classification using VGG19 & Transfer Learning

Coral reefs are vital ecosystems that support marine biodiversity and provide benefits like coastal protection and fisheries. This project applies **Deep Convolutional Neural Networks** and **Transfer Learning with VGG19** to classify coral images into different categories for better monitoring and conservation.

---

## 📌 Features

* ✅ Uses **VGG19 pre-trained model** with fine-tuning
* ✅ Data Augmentation for robust training
* ✅ Early stopping & learning rate scheduling
* ✅ Evaluation with accuracy, confusion matrix, and classification report
* ✅ Visualizations of predictions and training curves

---

## 📂 Dataset

* Images of corals categorized into multiple classes.
* Preprocessed with resizing, normalization, and augmentation.
* Split into **train/validation/test** sets.

---

## 🏗️ Model Architecture

* **Base model:** VGG19 (ImageNet weights)
* **Custom layers:** Dense, Dropout, Batch Normalization
* **Optimizer:** Adam
* **Loss:** Categorical Crossentropy
* **Metrics:** Accuracy

---



## ▶️ Usage

1. Prepare dataset folder structure:

```
dataset/
│── train/
│   ├── class1/
│   ├── class2/
│── val/
│   ├── class1/
│   ├── class2/
│── test/
```

2. Run the notebook:

```bash
jupyter notebook corals_image_classification_using_vgg19.ipynb
```

3. For inference, load the trained model and predict:

```python
from tensorflow.keras.models import load_model
model = load_model('vgg19_coral_model.h5')
```

## 🔮 Future Improvements

* Expand dataset with more coral species
* Try EfficientNet/ResNet for comparison
* Deploy as a web-based coral monitoring tool

