# **Google Play Store Data Analysis**

Welcome to the **Google Play Store Data Analysis** project! This project explores, cleans, and analyzes data from the Google Play Store to uncover trends, patterns, and insights about apps. Below is a detailed walkthrough of the analysis process and the key findings.

---

## **Table of Contents**

1. [Project Overview](#project-overview)
2. [Data Preprocessing](#data-preprocessing)
   - Handling Outliers
   - Managing Missing Values
   - Fixing Data Types
3. [Key Analysis and Visualizations](#key-analysis-and-visualizations)
4. [Insights](#insights)
   - Expensive Apps
   - Genre Popularity
   - Free vs. Paid Apps
5. [Analytical Questions Answered](#analytical-questions-answered)
6. [Technologies Used](#technologies-used)

---

## **Project Overview**

The dataset contains details of apps available on the Google Play Store, including categories, ratings, prices, install counts, and more. The main goals of this project are:

- Clean and preprocess the data for analysis.
- Identify trends and patterns in app categories, prices, and ratings.
- Answer specific business questions using the dataset.

---

## **Data Preprocessing**

### **1. Handling Outliers**
- Identified extreme outliers in the **Rating** column (values above 5).
- Used the median to replace outliers, as the median is less sensitive to extreme values.

### **2. Managing Missing Values**
- Missing values in columns such as **Rating**, **Size**, and **Type** were imputed using appropriate measures (median, mode, or mean).
- Treated entries with "Varies with device" in the **Size** column as NaN.

### **3. Fixing Data Types**
- Converted **Price** and **Installs** columns to numeric types after cleaning non-numeric characters.
- Transformed the **Last Updated** column into a datetime format for easier analysis.
- Split the **Android Version** column into two new columns: `Start Android Ver` and `End Android Ver`.

---

## **Key Analysis and Visualizations**

### **Rating Distribution**
- Visualized the distribution of app ratings using histograms and boxplots.
- Found that the data is slightly left-skewed but within an acceptable range.

### **Size Analysis**
- Treated missing values in the **Size** column with the mean size and converted all sizes into bytes for consistency.

### **Price Analysis**
- Analyzed the **Price** column and identified that most apps are free, with a few highly-priced apps.

### **Category Dominance**
- Used a pie chart to show that **ART_AND_DESIGN** is the most dominant app category.

### **Android Version Compatibility**
- Created a function to calculate the number of apps compatible with Android versions 4.x.

---

## **Insights**

### **1. Most Expensive App**
- The most expensive app is **`[APP_NAME]`**, priced at $400, from the **Lifestyle** category.

### **2. Genre Popularity**
- The genre with the highest number of apps is **`[GENRE_NAME]`**.

### **3. Free vs. Paid Apps**
- Free apps dominate the dataset, accounting for nearly **93%** of all apps.
- Free apps tend to be larger in size than paid apps on average.

### **4. Correlation Insights**
- The correlation between **Rating**, **Size**, and **Price** is weak due to the dataset's heavy bias toward free apps.

---

## **Analytical Questions Answered**

1. **What is the most expensive app on the Play Store?**
   - The app priced at $400 is **[APP_NAME]**.

2. **Which genre has the highest number of apps?**
   - The genre with the highest number of apps is **[GENRE_NAME]**.

3. **What is the average size of free vs. paid apps?**
   - Free apps: **[SIZE_FREE] Bytes**
   - Paid apps: **[SIZE_PAID] Bytes**

4. **What are the top 5 most expensive apps with a perfect rating (5)?**
   - [List of top 5 apps with prices and ratings.]

5. **What is Google's estimated revenue from apps with 5,000,000+ installs?**
   - Estimated revenue: **$[REVENUE]** (assuming a 30% cut).

6. **How many apps are compatible with Android version 4.x?**
   - There are **[COMPATIBLE_APPS]** apps compatible with Android version 4.x.

---

## **Technologies Used**

- **Python Libraries:**
  - `numpy`, `pandas`, `matplotlib`, `seaborn`, `plotly.express`
- **Data Cleaning Techniques:**
  - Imputation (mean/median/mode)
  - Outlier handling
  - Data type transformations
- **Visualization Tools:**
  - `matplotlib`, `seaborn`, and `plotly` for insightful visualizations.

---

### **Visualize the Code and Outputs**

To reproduce the analysis, clone the repository and run the Jupyter notebook containing the code. The dataset can be found [here](#).

### **Author**

Created by **[Your Name]**, passionate about data science and visualization. Connect with me on [GitHub](https://github.com/Hosam-emam).

---

### **License**

This project is licensed under the MIT License. Feel free to use and modify the code as per your requirements.

---

