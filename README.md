# 📊 Student Performance Analysis

> An Exploratory Data Analysis (EDA) project that analyzes student performance across Mathematics, Reading, and Writing using Python. This project explores how factors such as gender, parental education, and race/ethnicity influence academic performance through data cleaning, statistical analysis, and visualizations.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Dataset Information](#-dataset-information)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Data Preprocessing](#-data-preprocessing)
- [Exploratory Data Analysis](#-exploratory-data-analysis)
- [Visualizations](#-visualizations)
- [Key Insights](#-key-insights)
- [How to Run the Project](#-how-to-run-the-project)
- [Future Improvements](#-future-improvements)
- [License](#-license)

---

# 📖 Project Overview

Student performance is influenced by several demographic and educational factors. This project performs an Exploratory Data Analysis (EDA) on the **Students Performance Dataset** to identify meaningful trends and relationships between student scores and factors such as:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course

The analysis includes data validation, preprocessing, descriptive statistics, and insightful visualizations that help understand patterns in academic performance.

---

# 🎯 Objectives

- Perform data cleaning and preprocessing.
- Validate the dataset for missing and invalid values.
- Analyze score distributions.
- Compare student performance by gender.
- Study the impact of parental education on academic scores.
- Compare average scores across race/ethnicity groups.
- Identify the top-performing students.
- Present findings using informative visualizations.

---

# 📂 Dataset Information

The dataset consists of **1000 student records** and includes the following features:

| Feature | Description |
|----------|-------------|
| Gender | Student Gender |
| Race/Ethnicity | Student Group (A–E) |
| Parental Level of Education | Highest education level attained by parents |
| Lunch | Standard or Free/Reduced Lunch |
| Test Preparation Course | Completed or None |
| Math Score | Mathematics score (0–100) |
| Reading Score | Reading score (0–100) |
| Writing Score | Writing score (0–100) |

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# 📁 Project Structure

```text
Student-Performance-Analysis/
│
├── Analysis.ipynb
├── StudentsPerformance.csv
├── README.md
└── visuals/
    ├── distribution_math_scores.png
    ├── gender_scores.png
    ├── parental_education.png
    └── race_ethnicity.png
```

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Loaded the dataset using Pandas
- Examined dataset dimensions
- Checked column data types
- Generated descriptive statistics
- Checked for missing values
- Validated score ranges (0–100)
- Checked for duplicate records
- Verified absence of negative scores
- Created a new feature:

```python
df["average score"] = df[
    ["math score", "reading score", "writing score"]
].mean(axis=1)
```

This new feature represents the overall academic performance of each student.

---

# 📊 Exploratory Data Analysis

The analysis answers several important questions:

- How are Mathematics scores distributed?
- Which gender performs better in each subject?
- Does parental education influence student performance?
- Which race/ethnicity group performs the best?
- Who are the top-performing students?

---

# 📈 Visualizations

## 1️⃣ Distribution of Math Scores

The histogram below illustrates the distribution of Mathematics scores among students.

![Distribution of Math Scores](visuals/distribution_math_scores.png)

### Insights

- Scores approximately follow a normal distribution.
- Most students scored between **55 and 80**.
- Very few students scored below **30**.

---

## 2️⃣ Average Scores by Gender

This bar chart compares average scores across Mathematics, Reading, and Writing for male and female students.

![Average Scores by Gender](visuals/gender_scores.png)

### Insights

- Female students perform better in **Reading** and **Writing**.
- Male students slightly outperform females in **Mathematics**.
- Reading and Writing exhibit a more noticeable gender difference.

---

## 3️⃣ Parental Education vs Student Performance

This visualization explores the relationship between parental education level and student performance.

![Parental Education vs Student Performance](visuals/parental_education.png)

### Insights

- Students whose parents hold **Master's Degrees** have the highest average scores.
- Academic performance generally improves as parental education increases.
- Students whose parents completed only high school tend to have comparatively lower average scores.

---

## 4️⃣ Average Performance by Race/Ethnicity

The pie chart illustrates the average performance across different race/ethnicity groups.

![Race/Ethnicity Analysis](visuals/race_ethnicity.png)

### Insights

- Group **E** has the highest average academic performance.
- Group **A** records the lowest average score.
- Performance differences among groups are moderate.

---

# 🏆 Top Performing Students

Student performance was ranked based on the overall average score calculated from Mathematics, Reading, and Writing.

The notebook identifies the **Top 5 highest-performing students** based on this metric.

---

# 📌 Key Insights

- Student scores are approximately normally distributed.
- Female students perform better in Reading and Writing.
- Male students perform slightly better in Mathematics.
- Higher parental education is associated with better academic performance.
- Students from Group E achieved the highest average scores.
- The dataset contains no major missing values or invalid score entries.

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Student-Performance-Analysis.git
```

## 2. Navigate to the Project Directory

```bash
cd Student-Performance-Analysis
```

## 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## 4. Launch Jupyter Notebook

```bash
jupyter notebook Analysis.ipynb
```

---

# 📌 Future Improvements

- Correlation Heatmap
- Boxplots for Outlier Detection
- Pairplots for Feature Relationships
- Interactive Dashboard using Plotly
- Machine Learning Model to Predict Student Performance
- Feature Importance Analysis

---

# 🤝 Contributing

Contributions are welcome.

If you'd like to improve this project:

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Push to your branch.
5. Open a Pull Request.

---

# 📜 License

This project is intended for educational and learning purposes.

---

# 👨‍💻 Author

**Student Performance Analysis using Exploratory Data Analysis (EDA)**

Developed using **Python, Pandas, Matplotlib, and Seaborn** to analyze student academic performance and generate meaningful insights through data visualization.

---

## ⭐ If you found this project helpful, consider giving it a star on GitHub!
