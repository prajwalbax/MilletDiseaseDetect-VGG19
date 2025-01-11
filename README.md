# Disease Detection in Finger Millet (Ragi) Plant Using VGG19

## Overview
Finger millet (locally known as **Ragi**) is a vital crop for millions due to its nutritional and ecological benefits. However, diseases affecting finger millet can drastically reduce yield and threaten food security. This project focuses on developing a **disease detection system** using **VGG19**, a state-of-the-art Convolutional Neural Network (CNN), to assist farmers and researchers in identifying diseases early and accurately.

---

## Features
- **State-of-the-Art CNN**: Leveraging the power of **VGG16** with transfer learning to classify diseases in finger millet plants.
- **High Accuracy**: Tailored fine-tuning and data augmentation strategies ensure precise disease detection.
- **User-Friendly Interface**: An intuitive interface for real-time disease diagnosis.
- **Scalable Solution**: Designed to be extensible for other crops and regions.

---

## Dataset
The dataset consists of high-quality images of finger millet plants captured under various conditions. The dataset is preprocessed with techniques such as:
- **Image Resizing**: Standardized to the input size of 224x224 for VGG19.
- **Data Augmentation**: Rotation, flipping, and brightness adjustments to simulate diverse field conditions and reduce overfitting.

---

## Methodology
### 1. **Model Architecture**
The VGG19 model, pre-trained on ImageNet, serves as the base model. Key steps include:
- Removing the top classification layer.
- Adding custom dense layers with **Global Average Pooling**.
- Incorporating **Batch Normalization** and **Dropout** to prevent overfitting.

### 2. **Transfer Learning**
The pre-trained weights of VGG19 are fine-tuned to specialize in recognizing diseases in finger millet plants.

### 3. **Training Process**
- Optimizer: **Adam** with a learning rate of 0.0001.
- Loss Function: **Categorical Crossentropy** for multi-class classification.
- Metrics: Accuracy.

### 4. **Evaluation**
The model was evaluated on a validation set with metrics such as:
- Accuracy

---

## Results
- **Accuracy**: Achieved **86.7%** accuracy on the validation set.
- **Insights**: DenseNet performed better in earlier trials, but VGG16 showed comparable results with lower computational requirements.

---

## How to Use
### 1. **Prerequisites**
Ensure you have the following installed:
- Python 3.7+
- TensorFlow
- OpenCV
- Flask/Streamlit (for the user interface)

### 2. **Steps to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/prajwalbax/MilletDiseaseDetect-VGG19.git
   ```
2. Navigate to the project directory:
   ```bash
   cd ragi-disease-detection
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the model:
   ```bash
   python app.py
   ```
5. Access the web app:
   Open your browser and navigate to `http://localhost:5000`.

---
## List of disease detected:

1. Smut 
2. Seedling
   
![IMG-20240822-WA0001](https://github.com/user-attachments/assets/9844efc6-7a08-4ac5-b1bd-5ae396ce52c3)

3. Healthy
4. Downy Mildew
   
![IMG-20240822-WA0002](https://github.com/user-attachments/assets/ac09d1b5-f93a-4632-b249-0c4b5ae4a7e7)

5. Wilt
6. Mottle streak

![IMG-20240822-WA0003](https://github.com/user-attachments/assets/bcb0ae2b-b6eb-48fd-bae4-b96db735c658)



## Applications
- **Farmers**: Empower smallholder farmers with a tool to identify diseases early, reducing crop loss.
- **Researchers**: Aid agricultural researchers in understanding disease patterns.
- **Agricultural Extension Services**: Enhance extension officers' capacity to assist farmers.

---

## Future Work
- Expand the model to include more diseases and other crops.
- Incorporate Explainable AI (XAI) for better insights into predictions.
- Develop a mobile application for easier field use.

---

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a pull request.

---

## Acknowledgments
Special thanks to:
- The farmers and agricultural communities for their invaluable insights.
- Open-source contributors and the TensorFlow community for providing tools and resources.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
For questions, feedback, or collaboration, feel free to reach out:
- **Email**: prajwalbax@gmail.com
- **LinkedIn**: [prajwalbax](https://www.linkedin.com/in/prajwal-bax/)
- **GitHub**: [prajwalbax](https://github.com/prajwalbax)

Let's empower sustainable agriculture together!

