# 🧾 GST Fraud Detection – Hackathon Project
This project was developed for a hackathon focused on GST (Goods and Services Tax) fraud detection using machine learning. The goal is to classify whether given GST transactional records are fraudulent based on the provided features.

📁 Project Structure
nginx
Copy
Edit
gst hackathon project/
├── hackathon.ipynb                # Main notebook
├── Train_60/                      # Contains training data (X and Y)
├── Test_20/                       # Contains test data and checksum utilities
│   ├── X_Test_Data_Input.csv
│   ├── Y_Test_Data_Target.csv
│   ├── checksum.py
│   ├── SHA_256.txt
│   └── Instructions.txt
⚙️ Technologies Used
Python

Pandas, Matplotlib, Seaborn

Scikit-learn (RandomForestClassifier, preprocessing, metrics)

📊 Workflow Overview
Data Loading:

Training and test datasets are read using pandas.

Preprocessing:

Power transformation is applied to normalize feature distribution.

Feature selection is performed using mutual_info_classif.

Modeling:

A Random Forest Classifier is trained on the processed data.

Evaluation:

Accuracy, confusion matrix, classification report, and ROC-AUC are computed.

Plots like confusion matrix and ROC curve are generated.

Testing:

The trained model is evaluated on the provided test dataset (Test_20).

Test data integrity is verified via checksum.py.

📌 How to Run
Clone the repository.

Install dependencies:pip install pandas scikit-learn matplotlib seaborn


bash
Copy
Edit
pip install pandas scikit-learn matplotlib seaborn
Open hackathon.ipynb in Jupyter and run all cells.

(Optional) Use checksum.py in Test_20 to validate data integrity.

🧪 Evaluation Metrics
Accuracy Score

Classification Report

Confusion Matrix

ROC Curve and AUC Score

Mean Squared Error

