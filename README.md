# Diabetic Retinopathy Detection

This repository contains an implementation of Diabetic Retinopathy (DR) Detection using deep learning models, specifically EfficientNet and ResNet34. The goal is to develop an automated classification system that can assist healthcare professionals in detecting DR severity levels.

## 📌 Project Overview

**Diabetic Retinopathy** (DR) is a serious complication of diabetes that can lead to vision impairment or blindness. Early detection is essential to prevent severe damage. This project employs deep learning models to classify retinal images into different DR severity levels.

## 🚀 Models Used

The following models were implemented and evaluated for DR classification:

- **EfficientNet:** Known for its balance between accuracy and efficiency, EfficientNet scales depth, width, and resolution to improve performance.

- **ResNet34:** A deep residual network that utilizes skip connections to preserve gradient flow and minimize vanishing gradient issues.

## 📂 Repository Structure

```bash
├── dr-detection-efficientnet.ipynb   # Jupyter notebook for EfficientNet model
├── dr-detection-resnet34.ipynb       # Jupyter notebook for ResNet34 model
├── DR_detection_report.pdf           # Detailed report on project findings
├── README.md                         # Project documentation
```

## 📊 Dataset

The models were trained and evaluated using the "EYEQ Dataset", which consists of high-resolution retinal images captured under various imaging conditions. Each subject has both left and right eye images, labeled accordingly.

Images are classified into five DR severity levels:

- 0 - No DR

- 1 - Mild

- 2 - Moderate

- 3 - Severe

- 4 - Proliferative DR

The dataset presents real-world challenges, including noise, variations in image quality, and differences in camera types. Robust algorithms must account for artifacts, blurriness, and varying exposures to ensure accurate predictions.

## 📌 Dataset Links:

GitHub Repository for EYEQ Dataset

Papers with Code - EYEQ Dataset

🔧 Methodology
**1. Data Processing:** Retinal images were preprocessed through resizing, normalization, and augmentation to enhance model robustness and improve generalization.

**2. Model Selection and Setup:** EfficientNet and ResNet34 were chosen for their strong performance in image classification. The architectures were adapted for multi-class DR classification, with final layers adjusted accordingly.

**3. Model Training:** Both models were trained using cross-entropy loss and the Adam optimizer with learning rate scheduling. Iterative improvements were made by adjusting training parameters.

**4. Validation and Testing:** The trained models were evaluated on validation and test sets using cross-validation techniques to ensure generalization and prevent overfitting.

**5. Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score, and ROC-AUC were used to assess model performance, focusing on balanced classification across DR severity levels.

**6. Result Comparison and Selection:** EfficientNet and ResNet34 were compared based on validation performance, with EfficientNet emerging as the top-performing model due to its superior accuracy and computational efficiency.

## 📈 Results

EfficientNet achieved a validation accuracy of **~81%**.

ResNet34 achieved a validation accuracy of **~80%**.

Both models demonstrated stable convergence, but EfficientNet slightly outperformed ResNet34 in classification tasks.

## 📌 Future Improvements

Implementing ensemble learning for better predictions.

Exploring advanced data augmentation techniques.

Improving model interpretability for better explainability in medical diagnostics.

## 📝 Report

For a detailed explanation of the project, refer to the DR_detection_report.pdf file being attached in the repository.

## 🏆 Contributors

1. Karan Naik

2. Abhishikt Mahajan

🔗 License

This project is open-source and available under the MIT License.
