# 🛡️ Malicious URL Detection API

## 📌 Overview
This project is a Flask-based API that uses a machine learning model (Random Forest Classifier) to classify URLs as benign, malicious, phishing, defacement, or malware. The model is trained using extracted URL-based features.

## ✨ Features
✅ Extracts various features from URLs (length, presence of special characters, IP addresses, etc.).  
✅ Uses a trained Random Forest Classifier to predict URL type.  
✅ Provides an API endpoint to check URL classification.  
✅ Returns the accuracy of the model along with the classification result.  

## 📂 Dataset
The dataset used is `malicious_phish.csv`, which contains labeled URL data for training and evaluation.

## 🛠️ Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/MdSaad07/Malicious-URL-detection-API.git
   cd Malicious-URL-detection-API
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## 📦 Dependencies
Ensure you have the following Python libraries installed:
```sh
pandas
flask
sklearn
urllib
re
tld
```
You can install them using:
```sh
pip install pandas flask scikit-learn tld
```

## 🚀 Usage
### Running the API
```sh
python app.py
```

### 🔗 API Endpoints
#### 🎯 Predict URL Type
- **Endpoint:** `/api/predict`
- **Method:** `POST`
- **Request Body (JSON):**
  ```json
  {
    "url": "http://example.com"
  }
  ```
- **Response (JSON):**
  ```json
  {
    "url": "http://example.com",
    "type": "benign",
    "Accuracy": 0.95
  }
  ```

## 📊 Model Training & Accuracy
The model is trained using extracted URL-based features. It evaluates prediction accuracy and displays classification performance using `classification_report` and `accuracy_score`.

## 📜 License
This project is licensed under the MIT License.

## 👨‍💻 Author
Developed with ❤️ by **Mohammed Saad Fazal**  
🔗 GitHub: [MdSaad07](https://github.com/MdSaad07)  

