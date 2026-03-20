# Train-and-test-data
# 🧪 Data Splitting: Training vs. Testing Sets

A Machine Learning model is only as good as its ability to generalize to new data. This repository demonstrates the industry-standard process of partitioning a dataset into **Training** and **Testing** sets using **Scikit-Learn**.

---

## 🛠️ The Validation Stack
* **Python**: Core logic.
* **Pandas**: For dataset management and feature selection.
* **Scikit-Learn**: Specifically the `train_test_split` utility and `LinearRegression` for verification.
* **Matplotlib**: To visualize the distribution of the split data.

---

## 📊 Project Workflow

### 1. The 80/20 Rule
* **Training Set (80%):** The data the model "studies" to learn the relationship between features and targets.
* **Testing Set (20%):** The "final exam" data that the model has never seen before, used to evaluate its true performance.

### 2. Implementation with `train_test_split`
* Used `test_size` to control the ratio of the split.
* Implemented `random_state` to ensure **reproducibility**—allowing the same split to be generated every time the code is run.

### 3. Model Verification
* Trained a **Linear Regression** model on the training set.
* Evaluated the model's accuracy on the testing set using the `.score()` method.
* Compared training accuracy vs. testing accuracy to check for **Overfitting** or **Underfitting**.

---

## 🧠 Why Split Data?
If we test a model on the same data it practiced on, it will likely have a perfect score but fail in the real world. Splitting data allows us to:
* **Measure Generalization:** See how the model performs on data it hasn't seen.
* **Detect Overfitting:** Identify if the model is too complex and capturing "noise" instead of patterns.
* **Optimize Hyperparameters:** Tune the model to achieve the best balance between bias and variance.

---

## 🚀 How to Run

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git](https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git)
