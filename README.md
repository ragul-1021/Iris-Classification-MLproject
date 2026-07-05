# 🤖 Machine Learning Project | Iris Classification using FastAPI

A Machine Learning project that classifies Iris flowers into three species using a Decision Tree Classifier. The trained model is deployed locally with FastAPI, allowing users to send flower measurements and receive predictions through a REST API.

---

## 📌 Project Overview

This project demonstrates the complete machine learning workflow:

- Load and explore the Iris dataset
- Train multiple machine learning models
- Compare model performance
- Save the trained model using Joblib
- Build a REST API using FastAPI
- Predict Iris flower species through API requests

---

## 🚀 Features

- Iris flower classification
- Multiple ML algorithm comparison
- FastAPI REST API
- Input validation using Pydantic
- Model serialization with Joblib
- Interactive Swagger UI documentation

---

## 🛠️ Tech Stack

- Python
- Scikit-learn
- FastAPI
- Uvicorn
- Joblib
- Pydantic
- NumPy

---

## 📂 Project Structure

```
iris-classification/
│
├── models/
│   └── iris_model.pkl
│
├── src/
│   ├── app.py
│   ├── train.py
│   ├── compare_models.py
│   └── save_model.py
│
├── requirements.txt
└── README.md
```

---

## 🧠 Machine Learning Workflow

### Dataset
- Iris Dataset (Scikit-learn)

### Algorithms Used

- K-Nearest Neighbors (KNN)
- Decision Tree Classifier
- Support Vector Machine (SVM)

### Model Selected

Decision Tree Classifier

Reason:
- High accuracy on the Iris dataset
- Easy to understand and visualize
- Fast prediction time

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/ragul-1021/Iris-Classification-MLproject.git
```

Navigate to the project

```bash
cd Iris-Classification-MLproject
```

Create a virtual environment

```bash
python -m venv myenv
```

Activate the virtual environment

### Windows

```bash
myenv\Scripts\activate
```

### Linux / macOS

```bash
source myenv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the API

```bash
uvicorn src.app:app --reload
```

Open Swagger UI

```
http://127.0.0.1:8000/docs
```

---

## 📥 API Endpoint

### POST /predict

Request

```json
{
    "sepal_length": 5.1,
    "sepal_width": 3.5,
    "petal_length": 1.4,
    "petal_width": 0.2
}
```

Response

```json
{
    "prediction": "setosa"
}
```

---

## 📊 Model Performance

| Model | Accuracy |
|--------|---------:|
| KNN | High |
| Decision Tree | High |
| SVM | High |

The Decision Tree model was selected for deployment due to its strong performance and simplicity.

---

## 📚 Concepts Learned

- Machine Learning Classification
- Data Splitting
- Model Training
- Model Evaluation
- KNN
- Decision Tree
- Support Vector Machine
- Joblib Model Serialization
- FastAPI
- REST APIs
- Pydantic Models
- Swagger Documentation

---

## 🎯 Future Improvements

- Deploy the API to a cloud platform
- Add prediction confidence scores
- Dockerize the application
- Add unit tests
- Build a frontend interface

---

## 👨‍💻 Author

**Ragul B**

Aspiring AI Engineer passionate about Machine Learning, FastAPI, and Artificial Intelligence.

---

## ⭐ If you found this project helpful

Please consider giving this repository a ⭐ on GitHub.
