# Eye Disease Detection Using Deep Learning

## Introduction
This project classifies various types of eye diseases using deep learning. The diseases are categorized into:
- **Normal**
- **Cataract**
- **Diabetic Retinopathy**
- **Glaucoma**

The model is trained using deep learning techniques and deployed as a web application using Flask.

## Technologies Used
- **Python**
- **TensorFlow & Keras** (Deep Learning Framework)
- **Flask** (Web Application Framework)
- **NumPy, Pandas, Matplotlib** (Data Processing & Visualization)

## Prerequisites
Ensure you have the following installed:
- **Python 3.7+**
- **Anaconda (optional)**
- **Required Libraries**:
  ```bash
  pip install numpy pandas matplotlib tensorflow keras flask
  ```

## Dataset & Preprocessing
- The dataset consists of images categorized into four disease classes.
- Images are resized to **299x299** for compatibility with the Xception model.
- Normalization is applied to scale pixel values between 0 and 1.

## Model Training
- **Pre-trained Model:** Xception
- **Approach:** Transfer Learning
- **Additional Layers:** Fully connected dense layers for classification
- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Metrics:** Accuracy

### Model Training Steps:
1. **Load and Preprocess Data**
2. **Configure ImageDataGenerator**
3. **Use Xception as a Feature Extractor**
4. **Train the Model**
5. **Save the Model (`xception.h5`)**

## Deployment Using Flask
- The trained model is deployed using Flask.
- Users can upload an eye image, and the model predicts the disease category.
- Flask serves the model's predictions through a web interface.

### **Running the Flask App**
```bash
python app.py
```

### **Endpoints**
- **`/`**: Home page for image upload

## Project Structure
```
Eye_Disease_Detection/
│── app.py            # Flask Application
│── xception.h5       # Trained Model
│── templates/
│   └── index.html    # Frontend UI
│── static/uploads/   # Uploaded Images
│── Model_Training+testing.ipynb  # Jupyter Notebook
└── README.md         # Documentation
```

## Future Improvements
- Enhance dataset with more images for better generalization.
- Implement Explainable AI (XAI) techniques to visualize predictions.
- Extend support to additional eye diseases.
- Deploy using cloud services (AWS, GCP, or Azure).

## Contributors
- **Rohit Kumar Yadav**
- **Devasheesh Upreti**
- **Palak Agrawal**
- **Rohan Dorbi**
---
This README provides a comprehensive guide to understanding and running the project.
