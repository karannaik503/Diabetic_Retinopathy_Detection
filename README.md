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

📊 Dataset

The models were trained and evaluated using the EYEQ Dataset, which consists of high-resolution retinal images captured under various imaging conditions. Each subject has both left and right eye images, labeled accordingly.

Images are classified into five DR severity levels:

0 - No DR

1 - Mild

2 - Moderate

3 - Severe

4 - Proliferative DR

The dataset presents real-world challenges, including noise, variations in image quality, and differences in camera types. Robust algorithms must account for artifacts, blurriness, and varying exposures to ensure accurate predictions.

📌 Dataset Links:

GitHub Repository for EYEQ Dataset

Papers with Code - EYEQ Dataset

🔧 Methodology

Data Preprocessing: Image resizing, augmentation, and normalization.

Model Training: Fine-tuning EfficientNet and ResNet34 with cross-entropy loss and Adam optimizer.

Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, and ROC-AUC were used to assess model performance.

Hyperparameter Tuning: Learning rates, batch sizes, and optimizers were fine-tuned for optimal performance.

📈 Results

EfficientNet achieved a validation accuracy of ~81%.

ResNet34 achieved a validation accuracy of ~80%.

Both models demonstrated stable convergence, but EfficientNet slightly outperformed ResNet34 in classification tasks.

📌 Future Improvements

Implementing ensemble learning for better predictions.

Exploring advanced data augmentation techniques.

Improving model interpretability for better explainability in medical diagnostics.

📝 Report

For a detailed explanation of the project, refer to the DR_detection_report.pdf file.

🏆 Contributors

Karan Naik

Abhishikt Mahajan

🔗 License

This project is open-source and available under the MIT License.
