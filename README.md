# 📩 SMS Spam Classification
**SMS Spam Classification** is a Machine Learning project that classifies SMS messages as either **Spam** or **Ham** (legitimate). The project implements and compares **three classification models** — Naive Bayes, Logistic Regression, and SVM — on the same dataset to evaluate the performance of each algorithm.

The entire pipeline (data preprocessing, training, evaluation, and an interactive demo) is presented in a single Jupyter Notebook, making it easy to follow each step of a text classification problem from the basics to more advanced techniques.

## 🚀 Key Features

- **Data Preprocessing**: Text cleaning (removing special characters, lowercasing), tokenization, and vocabulary building
- **Text Vectorization**: Converting messages into word-count vectors for model input
- **Naive Bayes (built from scratch)**: Computes prior and conditional probabilities using Bayes' theorem for classification
- **Logistic Regression (built from scratch)**: Trained using Gradient Descent with the sigmoid function
- **SVM (Linear SVC)**: Trained using `scikit-learn` for comparison against the two custom-built models
- **Model Evaluation**: Calculates Accuracy, Precision, Recall, and F1-score for each model
- **Result Visualization**: Compares models using bar charts and a radar chart
- **Interactive Demo**: Real-time message classification via a Gradio interface

## 🛠️ Technologies Used

| Category | Technology |
|---|---|
| Language | Python 3 |
| Environment | Jupyter Notebook / Google Colab |
| Data Processing | pandas, NumPy |
| Machine Learning | scikit-learn (LinearSVC, metrics) |
| Visualization | Matplotlib |
| Demo Interface | Gradio |

## 📊 Dataset

This project uses the **[SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection)** dataset — a collection of over 5,000 English SMS messages labeled as `spam` or `ham`, provided as a tab-separated (`.tsv`) text file.

The data is split as follows:

- **80%** for the training set
- **20%** for the test set

## ⚙️ Prerequisites

Before running this project, make sure you have the following installed:

- **Python** 3.8 or higher
- **Jupyter Notebook** or **Google Colab** (recommended, since the notebook was built to run on Colab)
- **pip** to install the required libraries

## 📦 Installation & Local Setup

**1. Clone the project**

```bash
git clone https://github.com/thaibinhhl2006/spam_classification.git
cd spam_classification
```

**2. Install the required libraries**

```bash
pip install pandas numpy scikit-learn matplotlib gradio
```

**3. Download the dataset**

Download the **SMSSpamCollection** file and place it in the same folder as the notebook (if running on Google Colab, the notebook will prompt you to upload the file directly via the `files.upload()` cell).

**4. Run the notebook**

Open `Spam_Classification.ipynb` with Jupyter Notebook or Google Colab and run the cells in order:

```bash
jupyter notebook Spam_Classification.ipynb
```

Or click the **"Open in Colab"** badge at the top of the notebook to run it directly in your browser without setting up an environment.

## 💡 Usage

The notebook is organized into the following steps:

1. **Load and explore the data** — read the SMS dataset and inspect its structure
2. **Split the dataset** — 80% training, 20% test
3. **Clean & vectorize the data** — build the vocabulary and the word-count matrix
4. **Train each model** — Naive Bayes → Logistic Regression → SVM
5. **Evaluate & compare** — print Accuracy, Precision, Recall, F1-score, and plot comparison charts
6. **Live demo** — enter any SMS message into the Gradio interface to see whether the model predicts Spam or Ham

Example of using the Naive Bayes classification function directly in the notebook:

```python
classify("Congratulations! You've won a free ticket to Bahamas! Call 0901234567 now to claim your prize!")
# -> "spam"

classify("Hey, are we still meeting for dinner tonight?")
# -> "ham"
```

## 🤝 Contributing

Contributions are always welcome! If you'd like to improve this project (adding a new model, optimizing preprocessing, enhancing the demo interface...), please follow these steps:

1. **Fork** this repository to your own account
2. Create a new branch for your changes
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes
   ```bash
   git commit -m "Add: ..."
   ```
4. Push the branch to your repository
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a **Pull Request** for review and merging

Found a bug or have an idea? Feel free to open an [Issue](https://github.com/thaibinhhl2006/spam_classification/issues).

## 👤 Authors

- Nguyễn Thái Bình
- Vũ Hoàng Dương
- Hà Đức Duy
- Lê Quang Lộc
<p align="center">
  Made with ❤️ by the development team
</p>
