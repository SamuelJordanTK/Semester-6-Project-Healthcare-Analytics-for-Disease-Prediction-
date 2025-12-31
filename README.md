---

# Healthcare Analytics For Disease Prediction Using Machine Learning

### B.Tech (Artificial Intelligence & Data Science) — 6th Semester Project

This project presents the design and implementation of a **web-based health analytics system** capable of predicting potential diseases from user-provided symptoms. The application integrates **Machine Learning**, **Flask-based web deployment**, and comprehensive health-related knowledge resources to serve as an accessible, informative, and interactive digital health assistant.

> **Disclaimer**
> This system is intended strictly for academic and learning purposes. It is not a substitute for professional medical diagnosis or consultation.

---

## Project Objectives

* Develop a **symptom-driven disease prediction model**
* Provide **accurate and explainable predictions**
* Offer users additional **knowledge resources**, including:

  * Disease description
  * Precautions
  * Suggested medications
  * Dietary recommendations
  * Workout / care guidance
* Demonstrate integration of **AI + Web Technologies** in healthcare applications

---

## Machine Learning Methodology

### Dataset

The model is trained using structured healthcare datasets containing:

* Symptom attributes
* Disease mappings
* Supportive clinical metadata

All datasets are organized in:

```
Data/
│
├── Training.csv
├── Symptom-severity.csv
├── description.csv
├── diets.csv
├── medications.csv
├── precautions_df.csv
└── workout_df.csv
```

### Model Training & Evaluation

Multiple machine learning algorithms were experimented with, including:

* Support Vector Classifier (SVC)
* Random Forest
* Gradient Boosting
* K-Nearest Neighbors
* Multinomial Naive Bayes

After evaluation, the **Support Vector Classifier (Linear Kernel)** was selected due to its **high predictive performance and robustness**.
The trained model is serialized using `pickle` (`svc.pkl`) for deployment.

---

## System Architecture

```
├── main.py                  # Flask Web Application
├── svc.pkl                  # Trained ML Model
├── templates/               # HTML Templates
├── static/                  # CSS / Assets
├── Data/                    # Centralized Dataset Folder
└── README.md
```

---

## Technologies Used

| Category         | Tools                       |
| ---------------- | --------------------------- |
| Programming      | Python                      |
| Web Framework    | Flask                       |
| Machine Learning | Scikit-Learn                |
| Data Processing  | Pandas, NumPy               |
| Frontend         | HTML, CSS (Jinja Templates) |

---

## Setup & Execution

### 1️⃣ Clone the Repository

```
git clone https://github.com/yourusername/Health-Analytics-and-Disease-Prediction.git
cd Health-Analytics-and-Disease-Prediction
```

### 2️⃣ Install Dependencies

 manually install Flask, Pandas, NumPy, Scikit-Learn

### 3️⃣ Run the Application

```
python main.py
```

---

## Functional Workflow

1️⃣ User enters symptoms (comma-separated)
2️⃣ System preprocesses & encodes symptoms
3️⃣ Machine Learning model predicts likely disease
4️⃣ System displays:

* Predicted disease
* Description
* Precautions
* Medication guidance
* Recommended diet
* Workout / care tips

---

## Application Pages

| Route        | Purpose                   |
| ------------ | ------------------------- |
| `/`          | Main prediction interface |
| `/about`     | Project overview          |
| `/contact`   | Contact page              |
| `/developer` | Developer profile         |
| `/blog`      | Health awareness content  |

---

## Academic Significance

This project demonstrates core competencies expected in B.Tech (AI & Data Science):

* Applied machine learning
* Model evaluation & deployment
* Data preprocessing and feature engineering
* Full-stack AI system development
* Practical application in digital healthcare

---

## Future Enhancements

* Multi-disease probability prediction
* Improved UI/UX
* REST API support
* Real-time dataset integration
* Deployment to cloud platforms
* Enhanced dataset diversity and clinical realism

---

## Developer

**B.Tech – Artificial Intelligence & Data Science**
6th Semester Project
Samuel Jordan Tatchum Komguem
Feel free to connect for collaboration, research discussions, or improvements.

---

##  Acknowledgment

This project is a contribution toward leveraging Artificial Intelligence for improved accessibility to healthcare knowledge and awareness.

---
