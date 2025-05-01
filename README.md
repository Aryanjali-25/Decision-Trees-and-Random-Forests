# Decision-Trees-and-Random-Forests
# IMDb Top 250 - Classification using Decision Tree and Random Forest

#This project demonstrates a machine learning classification task using the IMDb Top 250 Movies dataset.
#We train and evaluate decision tree and random forest classifiers to predict whether a movie is rated "High" (≥8.5) or "Low" (<8.5), based on features such as rank, year, and runtime.

---

## Dataset

- File: imdb_top_250.csv
- Source: IMDb Top 250 Movies
- Target Variable: Target (binary classification)
  - '1' = High Rated (Rating ≥ 8.5)
  - '0' = Lower Rated (Rating < 8.5)

### Features Used

| Feature   | Description            |
|-----------|------------------------|
| Rank      | Position in Top 250    |
| Year      | Year of release        |
| Runtime   | Movie duration (mins)  |

---

## steps

### 1. Train a Decision Tree Classifier and Visualize the Tree
- Used DecisionTreeClassifier.
- Visualized using plot_tree() to understand decision paths.

### 2. Analyze Overfitting and Control Tree Depth
- Evaluated accuracy at varying tree depths.
- Plotted training vs test accuracy to detect overfitting or underfitting.

### 3. Train a Random Forest and Compare Accuracy
- Trained `RandomForestClassifier` with 100 trees.
- Compared accuracy against Decision Tree results.

### 4. Interpret Feature Importances
- Extracted feature importances from the trained Random Forest model.
- Visualized using a barplot for intuitive understanding.

### 5. Evaluate Using Cross-Validation
- Performed 5-fold cross-validation on the Random Forest model.
- Reported average accuracy and individual fold scores.

---

## Model Evaluation

- Metrics Used:
  - Accuracy
  - Classification Report (Precision, Recall, F1-score)
  - Cross-validation accuracy

