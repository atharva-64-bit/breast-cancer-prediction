# 🩺 Breast Cancer Prediction SaaS Platform

An intelligent web-based SaaS solution designed for pathology labs and doctors to predict the presence and stage of breast cancer using machine learning, featuring secure license-based access and health recommendations.

---

## 🔍 Features

- ✅ Secure login system with license number & expiration validation
- 🔐 Automated license approval workflow (no manual verification needed)
- 🧠 Random Forest Classifier trained on the Wisconsin Breast Cancer Dataset
- 🔬 Predicts:
  - Whether the tumor is Benign or Malignant
  - The stage of breast cancer (Early, Intermediate, Advanced)
- 💡 Provides personalized health recommendations based on stage
- 📄 Generates prediction reports
- 🧪 Designed for authorized pathology labs to securely access and use
- 🎨 Built using a clean and modern Streamlit UI

---

## 🚀 Tech Stack

| Layer            | Tools / Technologies                          |
|------------------|-----------------------------------------------|
| 🧠 Machine Learning | Random Forest Classifier, Scikit-learn         |
| 💾 Dataset         | Wisconsin Breast Cancer Dataset (30 features) |
| 🎛 UI              | Streamlit                                     |
| 🔐 Authentication  | Django for license validation + SQLite        |
| 📁 Database        | SQLite (no cloud database needed)             |
| 🌐 Deployment      | Local or Cloud-hosted (e.g., Streamlit Cloud) |

---

## 🔑 Workflow

1. Labs input their license number & expiration date
2. System verifies authenticity and expiration automatically
3. Once approved, the user is redirected to the main prediction platform
4. User inputs 30 numerical diagnostic features
5. Model predicts benign/malignant and cancer stage
6. Health recommendations shown based on predicted stage
7. Option to generate and save a report

---

## 📁 Project Structure

```

📦breast-cancer-prediction
┣ 📁 model/
┃ ┗ 📄 rf\_model.pkl
┣ 📁 pages/
┃ ┗ 📄 recommendation.py
┣ 📄 main.py
┣ 📄 login.py
┣ 📄 license\_verification.py
┣ 📄 requirements.txt
┣ 📄 README.md
┗ 📄 LICENSE

````

---

## ⚙️ How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/breast-cancer-prediction.git
   cd breast-cancer-prediction


2. Create virtual environment:

   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:

   * Windows:

     ```bash
     venv\Scripts\activate
     ```

   * Linux/Mac:

     ```bash
     source venv/bin/activate
     ```

4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Run the Streamlit app:

   ```bash
   streamlit run main.py
   ```

---

## 🧪 Sample Input Features

| Feature                   | Description                             |
| ------------------------- | --------------------------------------- |
| radius\_mean              | Mean of distances from center to points |
| texture\_mean             | Standard deviation of gray-scale values |
| ...                       | ...                                     |
| fractal\_dimension\_worst | "Worst" fractal dimension               |

(30 total diagnostic features)

---


## ✨ Author

Atharva Araj
GitHub: [@atharva-64-bit](https://github.com/atharva-64-bit)

---

## 🙌 Acknowledgements

* Wisconsin Breast Cancer Dataset from UCI ML Repository
* Streamlit for seamless UI creation
* Scikit-learn for robust model implementation

```


```

