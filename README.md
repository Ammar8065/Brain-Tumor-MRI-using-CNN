# Brain Tumor Classification using EfficientNetB0 & EfficientNetB1

## Overview
This project implements a deep learning model using EfficientNetB0 and EfficientNetB1 to classify brain tumors from MRI images. The model is trained to distinguish between four categories of brain tumors:
- Glioma
- Meningioma
- Pituitary
- No Tumor

## Dataset
The dataset used for training and evaluation is the **Brain Tumor MRI Dataset**, structured as follows:
```
Brain Tumor MRI Dataset/
  ├── Training/
  │   ├── Glioma/
  │   ├── Meningioma/
  │   ├── Pituitary/
  │   ├── No Tumor/
  ├── Testing/
      ├── Glioma/
      ├── Meningioma/
      ├── Pituitary/
      ├── No Tumor/
```
## 📂 Dataset & Preprocessing

Dataset: Brain MRI scans categorized into four tumor types.

Preprocessing steps:

Duplicate images removed for better dataset integrity.

Image resizing and normalization.

Data augmentation to improve generalization.

Splitting into training, validation, and test sets.




## 🔍 Model Architecture

We utilized **EfficientNetB0** and **EfficientNetB1**, which are lightweight and high-performing convolutional neural networks (CNNs). The models were fine-tuned on the dataset to achieve high accuracy while maintaining efficiency.

## Training Process
- Data was preprocessed and normalized.
- Images were augmented to improve generalization.
- The dataset was split into **training** and **validation** sets.
- The models were trained using **TensorFlow and Keras**.

## 📊 Performance & Evaluation
### EfficientNetB0
#### Training & Validation Accuracy!
![EfficientNetB0 (Train   Val acc )](https://github.com/user-attachments/assets/9d78bb5a-8a8f-43b4-b82b-d181e81f6e14)

#### Confusion Matrix
![EfficientNetB0 Confusion Matrix](https://github.com/user-attachments/assets/9337fc44-31d0-46b0-8bd1-5d00f2a3f4fb)

#### Random Predictions
![Random Prediction on images (EfficientNetB0)](https://github.com/user-attachments/assets/65a34103-8ec7-4ec8-ab95-34c831e33737)

### EfficientNetB1
### EfficientNetB1

#### Training & Validation Accuracy
![EfficientNetB1 Training & Validation Accuracy](./EfficientNetB1%20(Train%20%26%20Val%20acc.).png)

#### Confusion Matrix
![EfficientNetB1 Confusion Matrix](./EfficientNetB1%20Confusion%20Matrix.png)

#### Random Predictions
![Random Prediction on images (EfficientNetB1)](https://github.com/user-attachments/assets/f908a2e6-71c1-411e-9fa5-56b057a51d9e)

## 🚀 Results
- **EfficientNetB0** achieved a validation accuracy of **~80%**.
- **EfficientNetB1** performed significantly better, reaching **~98% accuracy**.
- The confusion matrices show strong performance in identifying tumor types correctly.

## Requirements
To run the model, install the required dependencies:
```bash
pip install tensorflow keras numpy matplotlib seaborn
```

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/brain-tumor-classification.git
   cd brain-tumor-classification
   ```
2. Run the training script:
   ```bash
   python train.py
   ```
3. Test the model on new images:
   ```bash
   python predict.py --image path/to/image.png
   ```

## Conclusion
EfficientNet models demonstrated strong classification capabilities for brain tumor MRI scans. **EfficientNetB1 outperformed EfficientNetB0**, making it the preferred choice for real-world applications.

## Future Improvements
- Experimenting with EfficientNetB2-B7 for better accuracy.
- Integrating Grad-CAM to visualize model decisions.
- Deploying the model as a web application for easy access.

---
**Author:** Ammar Shahid
