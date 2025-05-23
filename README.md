# 📰 Fake News Detection using Machine Learning and BERT

## 📌 Project Overview

This project aims to develop a robust fake news detection system using a combination of traditional machine learning models and advanced deep learning techniques (specifically, BERT). It explores multiple datasets and model combinations to improve the accuracy and reliability of fake news detection systems.

### 🔑 Key Highlights:
- **Traditional Machine Learning Models**: SVM, Random Forest, Naive Bayes.
- **Deep Learning Model**: BERT for text classification.
- **Hyperparameter Tuning**: GridSearchCV, Bayesian Optimization, PBT, Genetic Algorithms, Hyperband.
- **BERT + ML Integration**: Best-performing ML models (post-tuning) are combined with BERT for improved accuracy.

---

## 📂 Datasets Used

- **D1: ISOT Fake News Dataset** – Real and fake news articles.
- **D2: LIAR Dataset** – Labeled political statements.
- **D3: FakeNewsNet Dataset** – News articles with metadata and labels.

---

## 🏗️ Project Structure

```plaintext
Fake_News_Detection/
│
├── D1_Models/
│   ├── D1_BERT.ipynb      # BERT-based model for D1 dataset (without ML integration)
│   ├── D1_SVM.ipynb       # SVM model with hyperparameter tuning for D1 dataset and BERT + ML integration
│   ├── D1_RF.ipynb        # Random Forest model with hyperparameter tuning for D1 dataset and BERT + ML integration
│   └── D1_NB.ipynb        # Naive Bayes model with hyperparameter tuning for D1 dataset and BERT + ML integration
│
├── D2_Models/
│   ├── D2_BERT.ipynb      # BERT-based model for D2 dataset (without ML integration)
│   ├── D2_SVM.ipynb       # SVM model with hyperparameter tuning for D2 dataset and BERT + ML integration
│   ├── D2_RF.ipynb        # Random Forest model with hyperparameter tuning for D2 dataset and BERT + ML integration
│   └── D2_NB.ipynb        # Naive Bayes model with hyperparameter tuning for D2 dataset and BERT + ML integration
│
├── D3_Models/
│   ├── D3_BERT.ipynb      # BERT-based model for D3 dataset (without ML integration)
│   ├── D3_SVM.ipynb       # SVM model with hyperparameter tuning for D3 dataset and BERT + ML integration
│   ├── D3_RF.ipynb        # Random Forest model with hyperparameter tuning for D3 dataset and BERT + ML integration
│   └── D3_NB.ipynb        # Naive Bayes model with hyperparameter tuning for D3 dataset and BERT + ML integration
│
├── requirements.txt               # Python dependencies for the project
└── README.md                       # Project description and instructions

Each notebook:
- Trains models on a specific dataset.
- Applies multiple hyperparameter tuning strategies.
- Combines traditional models with BERT embeddings for enhanced accuracy.

---

🛠️ Installation

1. Clone the repository
    ```bash
    git clone <your-repository-url>
    cd Fake_News_Detection
    ```

2. Create a virtual environment
    ```bash
    python -m venv venv
    ```

3. Activate the virtual environment

    - On Windows:
    ```bash
    venv\Scripts\activate
    ```

    - On macOS/Linux:
    ```bash
    source venv/bin/activate
    ```

4. Install the dependencies
    ```bash
    pip install -r requirements.txt
    ```

🚀 Usage

1. Open any `.ipynb` file in the `D1_Models`, `D2_Models`, or `D3_Models` folders using Jupyter Notebook or JupyterLab.

Each notebook includes:

- **Preprocessing** of the respective dataset.
- **Model training** (Naive Bayes, SVM, Random Forest, or BERT).
- **Hyperparameter tuning** using various strategies (GridSearchCV, Bayesian Optimization, PBT, Genetic Algorithms, Hyperband).
- **Evaluation** with accuracy, F1-score, and confusion matrix.
- **Integration of the best ML model with BERT** (where applicable).


✅ Results

1. Traditional ML Models Perform Well on Balanced and Simple Datasets
    - Classical machine learning models like SVM, Naive Bayes, and Random Forest showed strong performance when applied to relatively clean and balanced datasets like ISOT, making them efficient for straightforward binary classification tasks.

2. BERT Excels in Complex and Real-World Scenarios
    - Deep learning models like BERT, with their ability to understand contextual and semantic nuances, outperformed traditional models on more complex datasets like LIAR and FakeNewsNet, proving their effectiveness in handling noisy, imbalanced, and real-world data.

3. A Hybrid Approach Yields the Most Robust Performance
    - Combining traditional ML models with deep learning techniques leverages the strengths of both approaches — efficiency and scalability from classical models, and deep language understanding from BERT — resulting in a more reliable and generalizable fake news detection system.


