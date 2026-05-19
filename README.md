# 🎬 Netflix Data Analysis using Python

## 📌 Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** of Netflix content using Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn. The analysis helps uncover valuable insights related to Netflix Movies and TV Shows including content distribution, ratings, countries, genres, release trends, duration analysis, and much more.

The project demonstrates practical skills in:

* Data Cleaning
* Data Understanding
* Data Visualization
* Exploratory Data Analysis (EDA)
* Feature Transformation
* Grouping & Aggregation
* Statistical Analysis

This project is ideal for showcasing:

* Data Analytics Skills
* Python Programming Skills
* Data Visualization Skills
* Portfolio Projects for GitHub
* MS Applications & Technical Profiles

---

# 📂 Dataset Information

The dataset contains Netflix Movies and TV Shows information including:

* Show ID
* Title
* Type (Movie / TV Show)
* Director
* Cast
* Country
* Date Added
* Release Year
* Rating
* Duration
* Genre (Listed In)
* Description

Dataset used: **Netflix Titles Dataset**

---

# 🛠️ Technologies & Libraries Used

## 🔹 Programming Language

* Python

## 🔹 Libraries Used

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np
```

---

# 📊 Project Workflow

## 1️⃣ Data Understanding

Performed initial exploration of the dataset using:

* `head()`
* `tail()`
* `shape`
* `dtypes`
* `info()`
* `describe()`
* `columns`

### Objectives

* Understand dataset structure
* Identify data types
* Explore categorical and numerical features
* Check dataset dimensions

---

## 2️⃣ Data Cleaning

Performed multiple preprocessing and cleaning operations:

### Cleaning Steps

* Checked missing values
* Checked duplicate records
* Converted `date_added` into datetime format
* Standardized column names into uppercase
* Verified unique values

### Example

```python
df['date_added'] = pd.to_datetime(df['date_added'])
df.columns = df.columns.str.upper()
```

---

## 3️⃣ Exploratory Data Analysis (EDA)

The project includes detailed analysis on Netflix content.

### 🔹 Content Type Analysis

* Movies vs TV Shows comparison
* Countplot visualization
* Pie chart distribution

### 🔹 Country Analysis

* Top countries producing Netflix content
* Country-wise content count

### 🔹 Ratings Analysis

* Most common audience ratings
* TV-MA content analysis

### 🔹 Release Year Analysis

* Content released over years
* Trend analysis
* Growth visualization

### 🔹 Genre Analysis

* Most popular genres
* Genre frequency analysis

### 🔹 Duration Analysis

* Distribution of movie durations
* Boxplot analysis
* Outlier detection

### 🔹 Director Analysis

* Top directors on Netflix

### 🔹 Correlation Analysis

* Heatmap visualization for numerical relationships

---

# 📈 Visualizations Included

The project contains multiple professional visualizations:

| Visualization       | Purpose                |
| ------------------- | ---------------------- |
| Countplot           | Movies vs TV Shows     |
| Pie Chart           | Content distribution   |
| Histogram           | Duration distribution  |
| Boxplot             | Outlier detection      |
| Line Plot           | Release trends         |
| Area Plot           | Netflix growth         |
| Bar Chart           | Top countries          |
| Horizontal Bar Plot | Top genres & directors |
| Heatmap             | Correlation analysis   |

---

# 📌 Key Insights Generated

## 🎥 Content Distribution

* Movies dominate Netflix compared to TV Shows.

## 🌍 Top Producing Countries

* Some countries contribute significantly more content.

## 📅 Content Growth

* Netflix content rapidly increased after 2015.

## ⭐ Audience Ratings

* TV-MA is one of the most common ratings.

## 🎭 Popular Genres

* Documentaries and entertainment genres are highly frequent.

## ⏳ Duration Trends

* Most movies fall within a common duration range.

---

# 📷 Sample Visualizations

## Movies vs TV Shows

```python
sns.countplot(x='TYPE', data=df)
plt.title("Movies vs TV Shows")
plt.show()
```

## Ratings Distribution

```python
plt.figure(figsize=(12,6))
sns.countplot(
    y='RATING',
    data=df,
    order=df['RATING'].value_counts().index
)
plt.title("Ratings Distribution")
plt.show()
```

## Correlation Heatmap

```python
sns.heatmap(
    df.corr(numeric_only=True),
    annot=True
)
plt.title("Correlation Heatmap")
plt.show()
```

---

# 🚀 Project Features

✅ Data Cleaning & Preprocessing
✅ Real-world Dataset Analysis
✅ Professional Visualizations
✅ GroupBy Operations
✅ Pivot Tables
✅ Statistical Insights
✅ Trend Analysis
✅ Correlation Analysis
✅ Beginner to Intermediate Level Project

---

# 📚 Concepts Covered

## Python Concepts

* Data Structures
* Functions
* Data Manipulation
* Aggregation
* Filtering
* Sorting
* Ranking

## Pandas Concepts

* DataFrames
* GroupBy
* Pivot Tables
* Missing Value Handling
* Datetime Conversion
* Explode Function
* Ranking Functions

## Visualization Concepts

* Countplots
* Histograms
* Boxplots
* Heatmaps
* Pie Charts
* Area Charts
* Bar Graphs
* Line Charts

---

# 🎯 Learning Outcomes

After completing this project, you will understand:

* How to perform real-world EDA projects
* How to clean and preprocess datasets
* How to create meaningful visualizations
* How to generate business insights from data
* How to work with Pandas efficiently
* How to use Seaborn and Matplotlib professionally

---

# 📁 Project Structure

```bash
📦 Netflix-Data-Analysis
 ┣ 📜 main.ipynb
 ┣ 📜 netflix1.csv
 ┣ 📜 README.md
```

---

# ▶️ How to Run the Project

## Step 1: Clone Repository

```bash
git clone <your-github-repository-link>
```

## Step 2: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

## Step 3: Run Jupyter Notebook

```bash
jupyter notebook
```


It demonstrates:

* Practical Data Analysis Skills
* Problem Solving
* Visualization Skills
* Data Cleaning Skills
* Python Proficiency

---

# 🙋‍♂️ Author

**Shlok Gadhave**

Passionate about:

* Data Analytics
* AI & Machine Learning
* Data Visualization
* Python Development
* Open Source Projects

---

# ⭐ If You Like This Project

If you found this project useful:

⭐ Star the repository
🍴 Fork the project
📢 Share with others




# 🔥 Final Conclusion

This project provides a complete hands-on implementation of Exploratory Data Analysis on Netflix data using Python. It covers data preprocessing, visualization, grouping, statistical analysis, and insight generation using professional libraries.

The project reflects strong foundational skills in Data Analytics and serves as an excellent portfolio project for students, aspiring data analysts, and AI/ML enthusiasts.
