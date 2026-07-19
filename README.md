# 🌸 FCR — Flower Classification Project

A Streamlit web app that predicts the species of an **Iris flower** using six different machine learning models, trained on the classic Iris dataset. Adjust the sliders for sepal/petal length and width, and see how each model votes — along with a final combined prediction.

## 🔗 Live Demo

[fcr-ml-collegebased-blazeo8.streamlit.app](https://fcr-ml-collegebased-blazeo8.streamlit.app/)

## 🧠 Models Used

The app loads six pre-trained models (`.pkl` files) and runs predictions from all of them side by side:

- Logistic Regression
- Naive Bayes
- Decision Tree
- Random Forest
- SVM
- KNN

## ⚙️ How It Works

1. The Iris dataset is loaded via `sklearn.datasets.load_iris`.
2. Users pick feature values (sepal length/width, petal length/width) using sliders in the sidebar.
3. On clicking **"Click here to Predict"**, all six models predict the flower class from the input.
4. Each model's prediction confidence is plotted in an interactive **Altair bar chart** for comparison.
5. The final prediction is the **mode** (most common answer) across all six models.

## 📁 Repository Structure

```
├── app.py                              # Streamlit app
├── Flower Classification Project.ipynb # Notebook: EDA, training & exporting the models
├── Logistic Regression.pkl
├── Naive Bayes.pkl
├── Decision Tree.pkl
├── Random Forest.pkl
├── SVM.pkl
├── KNN.pkl
├── download.png
├── requirements.txt
└── LICENSE
```

## 🚀 Running Locally

Clone the repo:

```bash
git clone https://github.com/BlazeO8/FCR_ML_College-based.git
cd FCR_ML_College-based
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the app:

```bash
streamlit run app.py
```

## 📦 Requirements

```
streamlit
pandas
numpy
scikit-learn
altair
seaborn
matplotlib
```

## 📓 Notebook

`Flower Classification Project.ipynb` contains the full workflow — data exploration, training each of the six models, evaluating them, and exporting the trained models as `.pkl` files used by `app.py`.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

Made with ❤️ using Streamlit
