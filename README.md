# MSCS-634-Lab2

# Lab 2: Classification Using KNN and RNN Algorithms

**Course:** MSCS-634-B01 – Advanced Big Data and Data Mining  
**Student:** Sandesh Pokharel  
**Lab Title:** Classification Using KNN and RNN Algorithms  
**Dataset:** Wine Dataset (from sklearn)

---

## 🔍 Purpose of the Lab

The objective of this lab is to explore and compare the performance of two distance-based classification algorithms—K-Nearest Neighbors (KNN) and Radius Neighbors (RNN)—using the Wine dataset from `sklearn`. The lab focuses on evaluating the impact of hyperparameters such as the number of neighbors (k) for KNN and the radius size for RNN on classification accuracy.

---

## ⚙️ Methods and Implementation

- The dataset was preprocessed with standard scaling to normalize features.
- KNN was tested with values of **k = 1, 5, 11, 15, 21**.
- RNN was tested with values of **radius = 350, 400, 450, 500, 550, 600**.
- Accuracy scores were recorded for each configuration.
- Matplotlib was used to visualize trends in classification accuracy.

---

## 📈 Key Observations and Insights

- **KNN Results:**  
  Accuracy improved steadily with increasing k and peaked at 100% for k = 11, 15, and 21. The KNN model was highly stable and performed well across all tested values.

- **RNN Results:**  
  Accuracy remained constant at 0.3889 across all radius values. This suggests that the model struggled to effectively classify due to poorly tuned radius values or a lack of sufficient neighbors within the given radius range.

- **Overall Comparison:**  
  KNN clearly outperformed RNN in terms of both accuracy and consistency. RNN was more sensitive to its parameter and less reliable on this dataset.

---

## 🧠 Challenges and Decisions

- **Radius Tuning in RNN:**  
  Selecting optimal radius values proved difficult, and most configurations led to the same poor accuracy. RNN's performance was less predictable compared to KNN.

- **Inline Interpretation:**  
  Based on previous feedback, extra effort was made to include explanatory markdowns and inline code comments to improve the clarity and self-sufficiency of the notebook.

- **Error Handling:**  
  The RNN section included try-except handling to account for model failures when no neighbors were found, ensuring smooth execution.

---

## 📁 Repository Contents

- `Lab2_KNN_RNN_Classifier.ipynb` – Jupyter Notebook with full implementation and commentary  
- `README.md` – This file  
- *(Optional)* `screenshots/` – Folder containing plot visuals if needed for documentation

---

## 🔗 How to Run

1. Clone the repository  
2. Activate your Python virtual environment  
3. Run the Jupyter Notebook using `jupyter notebook`  
4. Execute each cell in order to see results

---


