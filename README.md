# 🕵️‍♂️ Fraud Detection ML Project

Detect fraudulent transactions using machine learning. This repository includes a full working pipeline with data exploration, model training, and a Streamlit-based web app for deployment.

---

### 📂 Dataset

We use the **Fraud Detection Dataset** from Kaggle by Aman Ali Siddiqui, which includes over **6.3 million transaction records** labeled for fraud detection.

**Download link:**
[Fraud Detection Dataset on Kaggle](https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset)

---

### 📁 Repository Contents

\`\`\`
/
├── Fraud_Detection.ipynb ← Jupyter notebook: full EDA, preprocessing, modeling workflow
├── fraud_detection.py ← Streamlit app script for demoing the model
├── fraud_detection_pipeline.pkl ← Serialized trained ML pipeline (e.g., logistic regression)
├── README.md ← This documentation
└── .gitignore ← Files/folders to exclude from Git tracking
\`\`\`

---

### 🚀 Getting Started

#### 1. Clone the repository

\`\`\`bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
\`\`\`

#### 2. Download the dataset

Download the dataset from Kaggle (link above). Place the dataset file (e.g., \`AIML Dataset.csv\`) into the project root.


#### 3. Launch the Streamlit app

\`\`\`bash
streamlit run fraud_detection.py
\`\`\`

This will open the app in your browser, where you can test predictions using the trained model.

---


Here’s a preview of how the Streamlit app looks:
<img width="938" height="948" alt="app image" src="https://github.com/user-attachments/assets/88352eea-e072-4fae-b014-b9eb544c2c46" />



---

### 🔎 Project Workflow

**Exploratory Data Analysis (EDA)**

Initial data exploration and visualization to understand feature distributions, class imbalance, correlations, etc.

**Preprocessing & Modeling**

Setup of a processing pipeline using \`ColumnTransformer\` and scaling/encoding as needed.

Training of a \`LogisticRegression\` classifier with \`class_weight=\"balanced\"\`.

**Model Evaluation**

Metrics including precision, recall, confusion matrix, and accuracy were examined — recall for fraud is high (~94%), but precision is low (~2%).

**Model Serving in Streamlit**

The trained pipeline is saved as \`fraud_detection_pipeline.pkl\`, loaded in \`fraud_detection.py\`, which features interactive UI to input transaction data and get fraud predictions in real-time.
"


echo "Repository structure and files created successfully in '$REPO_NAME'!"
echo "Remember to replace '<your-username>' and '<repo-name>' in the README with your actual GitHub details."
