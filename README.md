# CS5710 Machine Learning — Homework 1

**University of Central Missouri**  
**Department of Computer Science **   
**Student:** Santhosh Reddy Kistipati **
**student id** 700776947

---

##  Assignment Overview
This repository contains my solutions for **Homework 1** of CS5710 — Machine Learning.  
The assignment covered theoretical problems, manual calculations, and a programming exercise on Linear Regression.  
This README provides explanations for each question and instructions to run the code.

---

##  Question Explanations

### **Q1 — Function Approximation by Hand**
- Dataset: (1,1), (2,2), (3,2), (4,5)  
- Tried two models:
  - Model 1: θ = (1,0) → Predictions matched more closely, MSE = 0.5  
  - Model 2: θ = (0.5,1) → Higher error, MSE = 1.125  
- **Answer:** Model 1 fits better since it achieves a lower Mean Squared Error. :contentReference[oaicite:0]{index=0}

---

### **Q2 — Random Guessing Practice**
- Cost function: \( J(θ) = 8(θ₁-0.3)² + 4(θ₂-0.7)² \)  
- Evaluations:  
  - J(0.1,0.2) = 1.32  
  - J(0.5,0.9) = 0.48  
- The guess (0.5,0.9) is closer to the true minimum (0.3,0.7).  
- **Explanation:** Random guessing is inefficient because it wastes many attempts, while gradient descent systematically moves toward the optimum. :contentReference[oaicite:1]{index=1}

---

### **Q3 — First Gradient Descent Iteration**
- Dataset: (1,3), (2,4), (3,6), (4,5)  
- Started with θ = (0,0), α = 0.01  
- Steps:
  1. Compute predictions at θ(0)  
  2. Residuals, ∑r, ∑xr  
  3. Gradient ∇J and update rule  
  4. Compare J(θ0) vs J(θ1)  
- Continued to second step θ(2), again comparing cost.  
- **Explanation:** Each iteration reduces error gradually, moving parameters closer to the least-squares solution. :contentReference[oaicite:2]{index=2}

---

### **Q4 — Compare Random Guessing vs Gradient Descent**
- Dataset: (1,2), (2,2), (3,4), (4,6)  
- Random guesses tried: (0.2,0.5), (0.9,0.1)  
  - Best guess → J = 1.935  
- First GD step from (0,0) → J ≈ 10.51  
- **Explanation:** A lucky random guess produced lower error than one GD step. However, gradient descent eventually beats random guessing as it converges systematically to the true solution. :contentReference[oaicite:3]{index=3}

---

### **Q5 — Recognizing Underfitting and Overfitting**
- Case: High training error + High test error  
- **Answer:** This is **underfitting** because the model is too simple to capture the data.  
- Fixes:  
  1. Increase model complexity (e.g., polynomial regression, more features).  
  2. Train longer or improve feature engineering. :contentReference[oaicite:4]{index=4}

---

### **Q6 — Comparing Models**
- Model A: Fits training data almost perfectly but fails on unseen data → **Overfitting** (low bias, high variance).  
- Model B: Performs poorly on both training and test → **Underfitting** (high bias, low variance).  
- Fixes:  
  - For Model A (overfit): regularization, pruning, more data.  
  - For Model B (underfit): increase complexity, add features, train longer. :contentReference[oaicite:5]{index=5}

---

### **Q7 — Programming Problem: Linear Regression**
- Task: Implement Linear Regression with both **Closed-form solution** and **Gradient Descent**.  
- Dataset: Synthetic, generated as \( y = 3 + 4x + ε \).  
- Results:  
  - Closed-form: intercept ≈ 2.69, slope ≈ 4.13  
  - Gradient Descent (η=0.05, 1000 iterations): converged to the same values.  
  - Loss curve shows GD steadily reducing error.  
- **Answer:** Gradient Descent converged to the same solution as the Normal Equation. :contentReference[oaicite:6]{index=6}

---

How to Run the Code
-->just click the gitup link and downlaod the python file and run in google colob : https://github.com/santhoshK12/Homework1ML/tree/main
