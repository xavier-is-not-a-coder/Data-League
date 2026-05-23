# 🏆 Data League Competition — Kharazmi University AI Association

Welcome to the official repository for the **Data League**, an intensive, multi-week data science competition organized by the **Practical Exploration Working Group** at the Kharazmi University AI Student Association. 

This repository contains the dataset, weekly challenges, and solution keys distributed to competing teams.

---

## 👥 Organization & Leadership

As a **Co-organizer**, I worked alongside a dedicated team of **6 members** to design, plan, and execute this event from start to finish. Our responsibilities included:
* **Curating & Cleaning the Datasets:** Sourcing the student performance data and modifying it to fit structured competition guidelines.
* **Designing the Weekly Roadmap:** Formulating analytical challenges that progressively tested participants from fundamental EDA to rigorous production-grade pipelines.
* **Developing Solution Keys:** Authoring reference notebooks (`Solution Keys`) utilized for objective scoring and evaluation of participant submissions.

---

## 📊 Dataset Overview: Student Performance Prediction

The core mission of the competition was to predict students' final numerical grades (**`G3`**) based on a rich array of demographic, social, and academic features.

### Feature Highlights:
* **Academic Metrics:** `G1` (first period grade), `G2` (second period grade), `failures`, `studytime`, `schoolsup`.
* **Social Factors:** `Dalc` & `Walc` (daily/weekend alcohol consumption), `freetime`, `goout`, `romantic`.
* **Demographics:** `school`, `sex`, `age`, `address` (Urban/Rural), `Medu`/`Fedu` (parents' education).

### Files Provided:
* `train.csv`: Contains all behavioral features along with the target column (`G3`) used to train models.
* `test.csv`: Contains features for testing. Participants must predict `G3` for these instances without seeing the ground truth.

---

## 🗺️ Competition Roadmap (Weekly Breakdown)

The league was structured into progressive modules to mirror real-world data science lifecycles:

### 📍 Week 1: Foundation & Deep Data Understanding
* **Focus:** Exploratory Data Analysis (EDA), identifying distribution anomalies, and basic preprocessing.
* **Core Tasks:**
  * Handling outliers in highly skewed variables (e.g., student `absences`).
  * Utilizing statistical transformations (Log transform, MinMax / Robust scaling).
  * Feature encoding strategies (One-Hot Encoding categorical structures).
  * **"Bug Hunt" Challenge:** Debugging broken boilerplate data code to teach defensive programming.

### 📍 Week 2: Cleaning & Modular Feature Engineering
* **Focus:** Transforming messy real-world data into reliable model inputs.
* **Core Tasks:**
  * Handling missing values systematically through statistical imputation.
  * Constructing complex custom features (e.g., compounding family background and socio-economic variables).
  * Introducing **Scikit-Learn Pipelines** to encapsulate transformations and prevent data leakage.
  * Transitioning from loose notebook cells into modular python scripts (`src/preprocessing.py`).

### 📍 Week 3: Modeling, Evaluation & Production
* **Focus:** Hyperparameter tuning, evaluating bias-variance tradeoffs, and compiling submissions.
* **Core Tasks:**
  * Training diverse regression algorithms (Linear Models, Tree-based architectures).
  * Analyzing metrics (RMSE, MAE) to evaluate model generalizability.
  * Formatting final predictions (`submission.csv`) under strict constraints (preventing index row inclusion, handling missing row shuffles).

---

## 🛠️ Tech Stack & Methods Used
* **Languages:** Python
* **Data Libraries:** Pandas, NumPy, SciPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn
* **Evaluation Metrics:** Root Mean Squared Error ($RMSE$)

---

## 🚀 How to Run the Infrastructure

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/data-league.git](https://github.com/your-username/data-league.git)
   cd data-league
