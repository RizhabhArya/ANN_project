# **Student Performance Prediction Using ANN (Regression)**
Using mendeley student data to implement ANN on it to preditct studentss academic performance based on features like attendance, study hours, scholarship (in total 31 features/columns)..

## **Project Overview**
The goal of this project is to **predict students’ final CGPA** (Cumulative Grade Point Average) based on various academic, personal, and lifestyle factors. By analyzing historical student data, the model can estimate how well a student might perform academically.

---

## **Dataset**
We used a dataset containing **1,200 student records** with the following types of information:

- **Personal information:** Age, gender, admission year, relationship status.
- **Academic background:** Previous SGPA, current semester, program enrolled, attendance.
- **Lifestyle and habits:** Hours spent studying, smartphone/computer usage, time spent on social media.
- **Extra details:** Skills, co-curricular activities, health conditions, family income.

The target variable is the **current CGPA** of the student.

---

## **Methodology**

1. **Data Cleaning and Preprocessing**
   - All missing numeric values were replaced with the average value for that column.
   - Missing categorical data was filled with the most frequent category.
   - Categorical data (like gender or program) was converted into a numerical format so the model can understand it.
   - The data was standardized to make all features comparable in scale.

2. **Model Used**
   - We used an **Artificial Neural Network (ANN)**, a type of machine learning model inspired by the human brain.
   - The model learns patterns between students’ features (like study hours or attendance) and their final CGPA.
   - The network had multiple layers that processed the data and predicted the CGPA as a continuous value.

3. **Training**
   - The dataset was split into a **training set** (to teach the model) and a **test set** (to evaluate its predictions).
   - The model was trained using the training data for multiple rounds (epochs) to improve its accuracy.
   - We used a **GPU** to make the training faster.

---

## **Results**
- **Mean Squared Error (MSE):** 0.120  
  *(Measures how far predictions are from actual CGPA; lower is better)*
- **R² Score:** 0.767  
  *(Shows how much of the CGPA variation the model can explain; 0.767 means about 77% of the variation is captured)*

**Interpretation:**  
The model predicts students’ CGPA fairly accurately. While it’s not perfect, it can give a **good estimate of student performance** based on their academic history and habits.

---

## **Visualizations**
1. **Loss Curve:** Shows how the model improved over training rounds.
2. **Predicted vs Actual CGPA:** A scatter plot comparing predicted values to real CGPA values.  
   - Points close to the diagonal line indicate accurate predictions.

---

## **Conclusion**
This regression model can help **universities and educators** estimate student performance early.  
It can be used for:

- Identifying students who might need additional support.
- Planning interventions to improve academic success.
- Providing insights into factors that influence CGPA.

