Gender Classification Data Visualization
📌 Project Overview
This project explores a dataset containing Height, Weight, Age, and Gender attributes. The goal is to visualize both categorical variables (Gender distribution) and continuous variables (Height, Weight, Age distributions) using Python, Pandas, Matplotlib, and Seaborn.
🎯 Objectives
  Visualize Gender distribution using bar charts.
  Explore Height, Weight, and Age distributions using histograms.
  Compare distributions across genders using grouped visualizations.
  Provide reusable code templates for data visualization in Google Colab or local environments.
🛠️ Tech Stack
  Python 3
  Pandas – data handling
  Matplotlib – plotting
  Seaborn – statistical visualization
  Google Colab – execution environment
📂 Dataset
The dataset includes the following columns:
  Gender → categorical variable (Male/Female)
  Height → continuous variable (in cm)
  Weight → continuous variable (in kg)
  Age → continuous variable (in years)
📊 Visualizations
1. Gender Distribution (Bar Chart)
python
sns.countplot(x='Gender', data=df, palette='Set2')
plt.title('Distribution of Gender in Population')
plt.show()

2. Continuous Variables (Histograms)
python
sns.histplot(df['Height'], bins=10, kde=True, color='skyblue')
sns.histplot(df['Weight'], bins=10, kde=True, color='lightgreen')
sns.histplot(df['Age'], bins=10, kde=True, color='salmon')

3. Gender-wise Comparison
python
sns.histplot(data=df, x='Height', hue='Gender', kde=True, palette='Set2')
sns.histplot(data=df, x='Weight', hue='Gender', kde=True, palette='Set2')
sns.histplot(data=df, x='Age', hue='Gender', kde=True, palette='Set2')
🚀 How to Run in Google Colab

    Upload the dataset:
    python
   from google.colab import files
uploaded = files.upload()
df = pd.read_csv("Gender_Classification_Data.csv")
📈 Sample Output

    Bar chart showing Male vs Female counts.

    Histograms showing Height, Weight, Age distributions.

    Overlaid histograms comparing Male vs Female distributions.

📌 Future Work

    Add boxplots to compare distributions more clearly.

    Perform statistical analysis (mean, median, variance by gender).

    Extend dataset with more demographic features.

👩‍💻 Author

Krithiga R

    B.Tech AI & Data Science, SRM Madurai
    Interests: Data Visualization, AI Ethics, Accessible Technology

