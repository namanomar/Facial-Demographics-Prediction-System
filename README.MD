# Facial Demographics Prediction System Using Deep Learning

## Overview
The **Facial Demographics Prediction System** is a deep learning-based project aimed at predicting age and gender from facial images. Using the **UTKFace dataset**, the project explores and fine-tunes state-of-the-art convolutional neural network (CNN) architectures to create an efficient and accurate model for demographic analysis.

---

## Features
- **Age and Gender Prediction**: Predicts age (numerical) and gender (binary: Male/Female) from facial images.
- **Pre-trained Models**: Evaluates and fine-tunes models like **VGG16**, **ResNet50V2**, **InceptionV3**, and **Xception** for optimized performance.
- **Data Preprocessing**: Implements a robust pipeline for image augmentation, resizing, batching, and normalization using **tf.data**.
- **Class Imbalance Management**: Detects and mitigates dataset imbalances for better generalization.
- **Performance Metrics**: Tracks loss and accuracy during training and validation using detailed plots.
- **Visualization Tools**: Uses tools like **Matplotlib** and **Plotly** to provide insights into data distribution and training progress.

---

## Dataset
**UTKFace Dataset**
- Contains over **20,000 facial images** annotated with age, gender, and ethnicity.
- Images vary in resolution, ethnicity, and demographics, making it suitable for robust model training.

### Data Preprocessing
- Images resized to a standard input shape for CNNs.
- Augmented with techniques like rotation, zooming, and flipping to enhance model generalization.

---

## Architecture and Methodology
1. **Pre-trained CNN Models**:
   - **VGG16**: Known for its simple and effective architecture.
   - **ResNet50V2**: Introduces skip connections for handling vanishing gradients.
   - **InceptionV3**: Utilizes factorized convolutions for computational efficiency.
   - **Xception**: Combines depthwise separable convolutions with residual connections.

2. **Optimization**:
   - Regularization using **dropout layers**.
   - Early stopping to prevent overfitting.
   - Data augmentation to increase model robustness.

3. **Evaluation Metrics**:
   - **Accuracy** for gender classification.
   - **MAE (Mean Absolute Error)** for age prediction.
   - Loss and accuracy plots to monitor training.

---

## Results
- Models evaluated based on validation accuracy and loss.
- Visualizations include:
  - **Data Distribution**: Pie charts and histograms for dataset analysis.
  - **Training Progress**: Line graphs of loss and accuracy.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/facial-demographics-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd facial-demographics-prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Download the **UTKFace dataset** and place it in the `data` folder.
https://www.kaggle.com/datasets/utkarshsaxenadn/age-and-gender-prediction-vgg16-resnet152v2


## Future Scope
- Extend functionality to include ethnicity prediction.
- Deploy the model as a web service using **Flask** or **FastAPI**.
- Explore transfer learning with larger datasets for improved accuracy.


---

## Acknowledgements
- **UTKFace Dataset**: [Link to Dataset](https://www.kaggle.com/datasets/utkarshsaxenadn/age-and-gender-prediction-vgg16-resnet152v2)
- **TensorFlow** and **Keras** frameworks for deep learning.
- Tutorials and open-source resources from the AI community.

---

