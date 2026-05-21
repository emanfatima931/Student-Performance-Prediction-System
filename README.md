# 🎓 Student Grade Predictor — Linear Regression (AI/ML Project)

A Python-based machine learning project that predicts a student's final grade using **Linear Regression (Normal Equation)**. Takes key academic factors as input and outputs a predicted grade, letter grade, and performance level.

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [How It Works](#how-it-works)
- [Input Parameters](#input-parameters)
- [Installation & Run](#installation--run)
- [Sample Output](#sample-output)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Author](#author)

---

## About the Project

This project applies **Supervised Machine Learning** to predict student academic performance. It uses the **Normal Equation** method to train a Linear Regression model on sample student data, then takes live user input to make a prediction — no external ML libraries like scikit-learn are used. The math is implemented from scratch using **NumPy**.

---

## Features

- ✅ Linear Regression implemented from scratch (Normal Equation)
- ✅ Predicts final grade as a percentage
- ✅ Converts predicted percentage to Letter Grade (A / B / C / D / F)
- ✅ Classifies performance level (Excellent / Good / Average / Poor)
- ✅ Input validation for assignment score
- ✅ No ML framework needed — pure Python + NumPy

---

## How It Works

The model is trained using the **Normal Equation**:

```
θ = (XᵀX)⁻¹ Xᵀy
```

Where:
- `X` = Feature matrix (attendance, study hours, assignment score, previous grade)
- `y` = Target vector (final grades)
- `θ` = Learned weights (coefficients)

Once trained, the model takes a new student's data as input and computes:

```
predicted_grade = X_new · θ
```

---

## Input Parameters

| Parameter | Description |
|-----------|-------------|
| `Attendance (%)` | Student's attendance percentage |
| `Study Hours / Week` | Average study hours per week |
| `Assignment Score` | Score out of 100 |
| `Previous Semester Grade` | Letter grade: A, B, C, D, or F |

---

## Grading Scale

| Percentage | Letter Grade | Performance Level |
|------------|--------------|-------------------|
| ≥ 85% | A | Excellent |
| ≥ 70% | B | Good |
| ≥ 50% | C | Average |
| ≥ 40% | D | Poor |
| < 40% | F | Poor |

---

## Installation & Run

### Prerequisites
- Python 3.x
- pip

### Install Dependencies

```bash
pip install pandas numpy
```

### Run the Project

```bash
python grade_predictor.py
```

---

## Sample Output

```
Enter the student's details:
Attendance Percentage: 88
Study Hours per Week: 12
Assignment Score (out of 100): 80
Previous Semester Grade (A, B, C, D, F): B

Predicted Final Grade: 82.45%
Letter Grade: B
Performance Level: Good
```

---

## Project Structure

```
📁 student-grade-predictor/
│
├── grade_predictor.py      # Main Python script
└── README.md               # Project documentation
```

---

## Technologies Used

- **Language:** Python 3
- **Libraries:** NumPy, Pandas
- **Algorithm:** Linear Regression (Normal Equation — from scratch)
- **Concepts:** Supervised Learning, Feature Engineering, Grade Classification

---

## Author

**Eman Fatima**  
BS Computer Science — Artificial Intelligence Project  
Arid Agriculture University Rawalpindi

> 📌 *Feel free to fork, star ⭐ the repo, or open a pull request with improvements!*
