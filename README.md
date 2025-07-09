# DataAnalysisWarmUpExercises
# Data Analysis Warm-Up  Basic data analysis notebook using Python and pandas. Covers filtering, sorting, value counts, apply(), and conditional selection. Built for practice and learning.

*📘 Jupyter Notebook*

*🛠️ pandas, Python*

By Harshavardhan Bommalata
# 📊 data_analysis_warmup_exercises

This project is a hands-on, beginner-friendly notebook created to strengthen data analysis skills using Python and pandas. It includes practical exercises on filtering, sorting, grouping, applying functions, and exploring data in tabular format.

---

## 📘 Project Overview

**Project Title**: Data Analysis Warm-Up Exercises  
**Level**: Beginner to Intermediate  
**Tool**: Jupyter Notebook  
**Libraries Used**: `pandas`, `numpy`

This project demonstrates foundational data analysis techniques using pandas. It simulates typical real-world scenarios such as working with student marks, filtering by conditions, applying custom functions, sorting, and summarizing data. This notebook serves as a warm-up or practice sheet for those starting in data science or data analysis with Python.

---

## 🎯 Objectives

1. Understand and apply basic pandas operations on tabular data.
2. Perform filtering and conditional selection (e.g., marks between 70–80).
3. Use sorting methods to order data by column values.
4. Apply custom functions using `.apply()` method.
5. Retrieve unique values and group data effectively.

---

## 🏗️ Project Structure

### 1. Data Setup

- Sample student data with columns like `name`, `gender`, and `marks`.
- Created using pandas DataFrame manually or by reading a file (if used).

```python
import pandas as pd

data = {
    'name': ['John', 'Alice', 'Bob', 'Ravi'],
    'gender': ['male', 'female', 'male', 'male'],
    'marks': [85, 92, 76, 67]
}

df1 = pd.DataFrame(data)
```

---

### 2. Data Analysis Tasks

#### ✅ Task 1: Filter Marks Between 70 and 80
```python
df1[(df1['marks'] >= 70) & (df1['marks'] <= 80)]
```

#### ✅ Task 2: Sort by Marks and Get Top 3
```python
df1.sort_values(by='marks', ascending=False).head(3)
```

#### ✅ Task 3: Apply Function to Halve Marks
```python
def halfmarks(x):
    return x // 2

df1['half_marks'] = df1['marks'].apply(halfmarks)
```

#### ✅ Task 4: Count Rows Where Gender is 'Male'
```python
df1[df1['gender'] == 'male'].count()
```

#### ✅ Task 5: Get Unique Genders
```python
df1['gender'].unique()
```

---

## 📊 Visualizations (Optional)

Basic bar charts or histograms can be added if needed:
```python
import matplotlib.pyplot as plt

df1['marks'].plot(kind='bar')
plt.title("Student Marks")
plt.show()
```

---

## 🔍 Summary & Learnings

- Practiced core pandas operations
- Learned how to filter, sort, and apply transformations to columns
- Reinforced understanding of indexing, boolean masking, and DataFrame manipulation

---

## 💻 How to Use

1. Clone the repository:
   ```bash
   https://github.com/harshavardhanBOMMALATA/DataAnalysisWarmUpExercises.git
   ```

2. Open the notebook:
   ```bash
   jupyter notebook DataAnalysisWarmUpExercises-checkpoint.ipynb
   ```

3. Run cells step-by-step and observe the outputs

---

## 📂 File Structure

```
📦 data_analysis_warmup_exercises
 ┣ 📓 DataAnalysisWarmUpExercises-checkpoint.ipynb
 ┗ 📄 README.md
```

---

## 👤 Author - HARSHAVARDHAN BOMMALATA

This project highlights practical pandas skills for beginner-level data analysis tasks. For more content on Python, SQL, or data science practice:

- **Instagram**: [@always_harsha_royal](https://www.instagram.com/always_harsha_royal/)  
- **LinkedIn**: [Connect on LinkedIn](https://www.linkedin.com/in/harshavardhan-bommalata-7bb9442b0/)  
- **Email**: hbommalata@gmail.com

---

**Thank you for viewing this project! Feel free to fork, clone, and explore the notebook for your own learning.**
