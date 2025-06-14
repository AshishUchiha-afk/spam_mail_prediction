#  📧 spam_mail_prediction
A machine learning model to classify emails as spam or not spam using natural language processing techniques.

## ⚙️ How to Run the Code Without Hassle in google colab

Follow the steps below to get started easily:

1. 📥 **Run the following cell in the notebook:**

   ```python
   from google.colab import files
   files.upload()
2.🔐 Upload your Kaggle token (kaggle.json) when prompted.

3.✅ Now the code is ready to run — all necessary permissions and access will be set up!

## ⚙️ How to Set Up the Project Locally (Kaggle API Method)

Follow these steps if you want to use the Kaggle API to download the dataset directly:

1. 🔑 **Get Your Kaggle API Credentials**  
   - Go to your [Kaggle Account Settings](https://www.kaggle.com/account)
   - Click on **"Create New API Token"**
   - This will download a file called `kaggle.json`

2. 📁 **Place the Token File**  
   - Move `kaggle.json` to the `.kaggle` folder:
     - On Windows: `C:\Users\<YourUsername>\.kaggle\kaggle.json`
     - On macOS/Linux: `~/.kaggle/kaggle.json`

3. 🧠 **Use the Following Code to Programmatically Download the Dataset**

   ```python
   import os
   import kaggle

   # Set Kaggle credentials (optional if kaggle.json is correctly placed)
   os.environ['KAGGLE_USERNAME'] = 'your_username'
   os.environ['KAGGLE_KEY'] = 'your_key'

   # Download and unzip the dataset
   kaggle.api.dataset_download_files('dataset', path='.', unzip=True)

---

## 📌 Project Highlights

- 🧠 Binary classification: **Spam (1)** or **Ham (0)**
- 🧹 Text preprocessing with lowercase conversion, punctuation removal, stopword filtering, etc.
- ✨ Feature extraction using **TF-IDF Vectorization**
- 🧪 Trained with models like **Naive Bayes**, **Logistic Regression**, or **SVM**
- 📈 Evaluated using accuracy score, confusion matrix, and classification report
- 💾 Saves the final model and vectorizer with Pickle for deployment

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- NLTK (or re module for text cleaning)
- TF-IDF Vectorizer
- Pickle

---
## 📁 Project Structure

spam_mail_prediction/
├── spam_mail_prediction.ipynb → Main notebook
├── spam.csv → Dataset file
├── spam_model.pkl → Trained ML model
├── vectorizer.pkl → TF-IDF vectorizer
└── README.md → Project documentation

---

## 📈 Model Evaluation

- Accuracy
- Confusion Matrix
- Classification Report

---

## 📌 Future Improvements

- Build a web app using Streamlit or Flask for live email input
- Integrate with email inboxes for real-time spam filtering
- Try deep learning models like LSTM or BERT for improved performance

---
