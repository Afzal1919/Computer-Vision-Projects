# Pneumonia Detection Using VGG19 CNN

## 📌 Overview
This project is a **web-based application** designed to detect **pneumonia** from chest X-ray images using a **deep learning model**. The model is built on the **VGG19** architecture and is served through a **Flask-based web interface**. Users can upload chest X-ray images, and the application will predict whether the image indicates **pneumonia** or is **normal**.

## 🚀 Features
- **🔍 Deep Learning Model**: Utilizes a **VGG19 Convolutional Neural Network (CNN)** pretrained on ImageNet and fine-tuned for pneumonia detection.
- **🌐 Web Application**: A **Flask-based** web app that allows users to upload images and receive predictions.
- **📊 Data Preprocessing**: Includes **image resizing (128x128 pixels)** and **data augmentation** techniques to enhance model performance.
- **📈 Model Training & Evaluation**: Uses **chest X-ray datasets**, advanced training strategies, and performance evaluation metrics.

## 📂 Project Structure
```
├── app.py                     # Main Flask application script
├── model_weights/
│   ├── vgg19_model_01.h5      # Pretrained model weights
├── templates/
│   ├── index.html             # Frontend template for the web app
├── uploads/                   # Directory for storing uploaded images
├── Pneumonia_detection_DL.ipynb  # Jupyter Notebook with data preprocessing, model training, and evaluation
├── requirements.txt            # List of dependencies
└── README.md                   # Project documentation
```

## ⚡ Installation
### 🛠 Prerequisites
Ensure you have the following installed:
- **Python 3.6 or higher**
- **Flask**
- **TensorFlow 2.18.0**
- **Keras 3.7.0**
- **OpenCV**
- **NumPy**
- **Pillow**

### 🔧 Steps to Set Up the Project
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Afzal1919/Pneumonia_Detection.git
   cd Pneumonia_Detection
   ```

2. **Create and activate a Python virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # For macOS/Linux
   venv\Scripts\activate  # For Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download the pretrained model weights:**  
   Download the `vgg19_model_01.h5` file from [this link](#) and place it in the `model_weights/` folder.

5. **Run the Flask app:**
   ```bash
   python app.py
   ```
   Access the application at at: **[http://127.0.0.1:5000/]**

## 🎯 Usage
1. **Launch the web application.**
2. **Upload a chest X-ray image** using the provided interface.
3. **Click the 'Predict' button** to receive a classification result (Normal/Pneumonia).

## 🏆 Model Training
The model was trained using the [**Chest X-Ray Images (Pneumonia) dataset**](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) from Kaggle, consisting of training, validation, and test sets.

### 🔍 Training Steps
- **📂 Data Loading**: The dataset is loaded and processed using **OpenCV**.
- **🖼 Data Augmentation**: Techniques such as **flipping, rotation, and shearing** are applied.
- **🧠 Model Architecture**: A **VGG19 model** with additional dense layers for classification.
- **⚙️ Training Process**: The model is compiled using the **SGD optimizer** and trained with **early stopping** and **learning rate reduction**.
- **📊 Evaluation**: The model is evaluated on **validation and test sets** for accuracy and loss.

## 🤝 Contributing
We welcome contributions! If you'd like to improve the project:
1. **Fork the repository** 📌
2. **Create a new branch** 🛠
3. **Make your changes** ✏️
4. **Submit a pull request** 🚀

## 📜 Acknowledgements
- The dataset used in this project was provided by **Paul Mooney on Kaggle**.
- The **VGG19 architecture** is sourced from the **Keras library**.

---
Feel free to ⭐ **star this repository** if you found it useful! 😊
