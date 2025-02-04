# Breast-Cancer-Diagnosis-Using-Gaussian-Na-ve-Bayes
This project implements a Gaussian Naïve Bayes classifier for diagnosing breast cancer using the Breast Cancer Wisconsin (Diagnostic) dataset. The classifier is tested under different noise levels to evaluate its robustness.

# Dataset

Source: UCI Machine Learning Repository
Features: 30 real-valued medical attributes (tumor cell characteristics).
Classes: Malignant (1) and Benign (0).
Implementation Details

🛠️ Steps

# Load the Dataset: Downloaded from UCI ML Repository.
Preprocess Data: Convert diagnosis labels ('M' -> 1, 'B' -> 0), remove unnecessary columns.
Train Naïve Bayes Model: Use GaussianNB() from sklearn.naive_bayes.
Test Model Performance: Evaluate accuracy and confusion matrix.
Add Noise: Inject zero-mean Gaussian noise with variances [50, 100, 200, 400, 800].
Analyze Results: Measure accuracy drop under noisy conditions.

# Results
Accuracy with noise variance 50: 0.9474
Accuracy with noise variance 100: 0.9474
Accuracy with noise variance 200: 0.9474
Accuracy with noise variance 400: 0.9386
Accuracy with noise variance 800: 0.9298

# Installation & Usage

#🔧 Setup Environment

# Clone this repository
git clone https://github.com/your-username/breast-cancer-naive-bayes.git
cd breast-cancer-naive-bayes

# Install dependencies
pip install -r requirements.txt

#🚀 Run the Model

python src/naive_bayes.py

📓 Run Jupyter Notebook

Without noise: High precision and recall.
With noise: Gradual decline in classification accuracy.

# Discussion

✅ Advantages of Naïve Bayes:

# Fast and efficient for high-dimensional datasets.

Works well even with small datasets.

Interpretable results.

# ❌ Limitations:

Assumes feature independence (not always true).

Sensitive to noise at extreme levels.

Zero-frequency problem (handled using Laplace smoothing).

# Future Improvements

Implement feature scaling to improve noise resilience.

Compare with Logistic Regression and SVM.

Explore feature selection techniques to remove redundant attributes.

# License

This project is open-source under the MIT License.

