# Task-7-Support-Vector-Machines
Task 7: Support Vector Machines
 Tools & Libraries Used
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---
Step-by-Step Implementation

### 🔹 **Step 1: Importing Required Libraries**
Imported all essential libraries for data handling, visualization, model training, and evaluation.

### 🔹 **Step 2: Load and Inspect the Dataset**
- Loaded the CSV using `pandas`
- Displayed the top rows and checked for null values
- Dropped unnecessary column (`id`)
- Converted target labels to numeric (`diagnosis`: M → 1, B → 0)

### 🔹 **Step 3: Feature Scaling**
- Applied `StandardScaler` to normalize features
- Scaling is important for SVM as it’s sensitive to feature magnitudes

### 🔹 **Step 4: Splitting the Dataset**
- Used `train_test_split` to split the data:
  - 80% for training
  - 20% for testing

### 🔹 **Step 5: Model 1 - SVM with Linear Kernel**
- Trained an SVM with `kernel='linear'`
- Made predictions and evaluated with:
  - Accuracy Score
  - Classification Report

### 🔹 **Step 6: Model 2 - SVM with RBF Kernel**
- Trained an SVM with `kernel='rbf'` for non-linear classification
- Evaluated performance as above

### 🔹 **Step 7: Hyperparameter Tuning**
- Used `GridSearchCV` to tune `C` and `gamma` for RBF SVM
- Performed 5-fold cross-validation
- Identified the best parameters and evaluated test accuracy

### 🔹 **Step 8: Cross-Validation**
- Performed cross-validation on the tuned model
- Reported individual fold scores and average accuracy

### 🔹 **Step 9: Confusion Matrix**
- Visualized true positives, false positives, true negatives, and false negatives
- Helped in understanding misclassification

